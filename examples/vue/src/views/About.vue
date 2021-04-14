<template>
  <div class="about">
    <h1>This is about page</h1>
    <div class="content">
      <div class="content-light"></div>
      <span class="content-text">已连接</span>
      <div class="content-img">
        <el-avatar src="https://cube.elemecdn.com/0/88/03b0d39583f48206768a7534e55bcpng.png"></el-avatar>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .about {
    color: #7265e6;
  }
  .content {
    height: 42px;
    width: 205px;
    background-color: #545C63;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  .content-light:before,
  .content-light:after {
    position: absolute;
    content: '';
    height: 18px;
    width: 18px;
    margin-left: -25px;
    margin-top: -10px;
    border-radius: 50%;
    background-color: #66C13A;
    animation: warn 1.5s ease-out 0s infinite;
  }
  .content-text {
    color: #66C13A;
    display: block;
  }
  .content-img {
    margin: 0 15px;
    text-align: right;
  }
  @keyframes warn {
    0% {
      transform: scale(0.5);
      opacity: 1;
    }

    30% {
      opacity: 1;
    }

    100% {
      transform: scale(1.4);
      opacity: 0;
    }
  }
</style>
