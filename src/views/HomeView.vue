<template>
  <div></div>
</template>

<script>
export default {
  created() {
    let myFirstPromise = new Promise((resolve, reject) => {
      setTimeout(function () {
        resolve("성공!"); // 와! 문제 없음!
      }, 3000);
    });
    console.log("테스트용 글");
    myFirstPromise.then((message) => {
      console.log(message);
    });
  },
};
</script>

<style scoped></style>
