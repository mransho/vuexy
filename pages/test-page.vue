<template>
  <div>
    <VCard title="Create Awesome 🙌">
      <VCardText>This is your second page.</VCardText>
      <VCardText> test </VCardText>
    </VCard>
  </div>
</template>
<script lang="ts" setup>
import { definePage } from "vue";
definePage({
  meta: {
    action: "read",
    subject: "AclDemo",
  },
});

const user = {
  action: "read" as const,

  // `subject` property type is `Subjects` ("src/plugins/casl/AppAbility.ts")
  subject: "Admin" as const,
};
</script>
