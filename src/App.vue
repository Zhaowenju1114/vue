<template>
  <div class="p">
    <div class="a">
      <input type="text" name="" placeholder="               搜索对话" />
    </div>
    <div id="app">
      <ul>
        <li>
          <img src="./assets/img/user1.png" alt="" />
        </li>
        <li class="b">
          <p>张三</p>
          <p>同学，请问你什么时候能到岗</p>
        </li>
        <li>
          <p></p>
          <p>18:00</p>
        </li>
      </ul>
      <p class="h"></p>
      <ul>
        <li>
          <img src="./assets/img/user2.png" alt="" />
        </li>
        <li class="b">
          <p>王五</p>
          <p>同学，不好意思我们已经招满人了...</p>
        </li>

        <li>
          <p></p>
          <p>17:00</p>
        </li>
      </ul>
      <p class="h"></p>
    </div>

    <div class="bth">
      <ul>
        <li>
          <div><img src="./assets/img/work.png" alt="" /></div>
          <p>工作</p>
        </li>
        <li>
          <div><img src="./assets/img/message.png" alt="" /></div>
          <p>消息</p>
        </li>
        <li>
          <div>
            <img src="./assets/img/mine.png" alt="" />
          </div>
          <p>我的</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
 
};
</script>

<style lang="less">
#app {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  ul {
    width: 95%;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    li:nth-of-type(3) {
      display: flex;
      align-content: space-between;
      flex-wrap: wrap;
      p {
        height: 20px;
        width: 100%;
      }
    }
  }
}
* {
  margin: 0;
  padding: 0;
}
.a {
  width: 100%;
  height: 70px;
  background-color: #00669a;
  display: flex;
  justify-content: center;
  align-items: center;
  input {
    height: 50%;
    width: 90%;
    outline: none;
    font-size: 18px;
    border-radius: 20px;
    background: url(../src/assets/img/search.png) no-repeat 8px 5px;
    background-color: aliceblue;
    background-size: 30px 30px;
  }
}

.b {
  width: 30%;
  height: 55px;
  flex: 0.8;
  display: flex;
  align-content: space-between;
  flex-wrap: wrap;
  p:nth-of-type(2) {
    font-size: 12px;
    width: 100%;
  }
}

.h {
  width: 80%;
  height: 1px;
  background-color: #626566;
}
.bth {
  width: 100%;
  position: fixed;
  bottom: 0px;
  display: flex;
  justify-content: center;
  ul {
    width: 80%;
    list-style: none;
    display: flex;
    justify-content: space-between;

    li {
      div {
        display: flex;
        justify-content: center;
        img {
          width: 45%;
          height: 45%;
        }
      }
      p {
        text-align: center;
      }
    }
  }
}
</style>
