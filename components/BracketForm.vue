<template>
  <UForm :schema="schema" :state="state" class="space-y-4" @submit="onSubmit">
    <UFormGroup label="Number Of Teams" name="numberOfTeams">
      <USelectMenu v-model="state.numberOfTeams" :options="teamSizes" />
    </UFormGroup>

    <UButton type="submit"> Submit </UButton>
  </UForm>
</template>


<script setup lang="ts">
import { z } from "zod"
import type { FormSubmitEvent } from "#ui/types"

// Python has better ways to create lists of numbers without having to type them out
const teamSizes = ["2", "4", "6", "8", "10", "12", "14", "16", "18", "20", "22", "24"]

const schema = z.object({
  numberOfTeams: z.string().refine((value) => teamSizes.includes(value))
})

type Schema = z.output<typeof schema>

const state = reactive({
  numberOfTeams: "4"
})

async function onSubmit(event: FormSubmitEvent<Schema>) {
  // Do something with data
  console.log(event.data)
}
</script>


