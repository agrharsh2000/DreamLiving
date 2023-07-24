<template>
  <button :class="buttonClass" type="button" @click="handleClick">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      required: true,
      default: "Button",
    },
    variant: {
      type: String,
      default: "primary",
    },
  },
  methods: {
    handleClick() {
      this.$emit("click");
    },
  },
  computed: {
    buttonClass() {
      return `my-button my-button--${this.variant}`;
    },
  },
};
</script>

<style scoped>
.my-button {
  padding-left: 16px;
  padding-right: 16px;
  padding-top: 8px;
  padding-bottom: 8px;

  font-size: 16px;
  font-weight: 400;
  border-radius: 99px;
  transition: all 0.3s ease;

  
}

.my-button--primary {
    background-color: #000000;
    color: #ffffff;
}
.my-button:hover {
      background-color: #ffffff;
      color: #000000;
    }
  

  .my-button--secondary {
    background-color: #ffffff;
    color: #000000;
 
  }
    .my-button:hover {
      background-color: #000000;
      color: #ffffff;
    }
  
</style>
