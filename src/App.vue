<template>
  <div
    class="w-full h-full my-4 flex flex-col flex-wrap items-center justify-center"
  >
    <Button color="bg-blue-400" hoverColor="bg-blue-900" value="Click Me!" />
    <Input type="text" />
    <Alert />
    <LoginForm />
  </div>
</template>

<script>
import Button from "./components/button.vue";
import Input from "./components/input.vue";
import Alert from "./components/alert.vue";
import LoginForm from "./components/loginform.vue";

export default {
  name: "app",
  components: {
    Button,
    Input,
    Alert,
    LoginForm
  }
};
</script>

<style lang="scss"></style>
