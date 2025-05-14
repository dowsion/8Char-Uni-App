<template>
  <u-divider bg-color="transparent" class="u-p-30" @click="handleClick">{{copyright()}}</u-divider>
</template>

<script setup>
import {APP_AUTHOR, APP_NAME} from "@/config";

const copyright = () => {
  let date = ` ${new Date().getFullYear()}`
  return `© ${date} ${APP_NAME} Powered by ${APP_AUTHOR}`
}

</script>
