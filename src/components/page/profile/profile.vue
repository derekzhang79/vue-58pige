<template>
  <div class="page bg-gray">
    <transition name="slide">
      <router-view class="child-view"></router-view>
    </transition>
    <div class="scroll-view">
      <header class="app-header header-fill">
        <div class="back" @click="goback">
          <i class="iconfont icon-fanhui"></i>
        </div>
        <div class="page-title">我的</div>
      </header>
      <section>
        <div class="content user">
          <div class="user-info">
            <span class="name">{{ user.name }}</span>
            <span class="phone">{{ user.phone }}</span>
          </div>
          <router-link :to="{name: 'info', params: {uid: user.id, name: user.name, phone: user.phone}}" tag="div" class="edit-button">修改资料</router-link>
        </div>
        <router-link to="/profile/shopEdit" tag="div" class="content shop">
          <span>我的店铺</span>
          <i class="iconfont icon-icon1"></i>
        </router-link>
      </section>
      <div class="tab-container">
        <header class="tab">
          <span class="tab-item tab-active">我的发布</span>
          <span class="tab-item">我的收藏</span>
        </header>
        <ul class="info-feeds tab-content">
          <router-link to="/detail" class="info-item" tag="li">
            <div class="icontent">
              <div class="title">水刺底仿猪皮革 无纺布底PU仿猪里皮</div>
              <div class="parameter">
                <div class="param-list left">
                  <div class="param-item">
                    <span class="value">黄牛皮</span>
                    <span class="param">品种</span>
                  </div>
                  <div class="param-item">
                    <span class="value">A级</span>
                    <span class="param">皮胚</span>
                  </div>
                  <div class="param-item">
                    <span class="value">0.7mm</span>
                    <span class="param">厚度</span>
                  </div>
                </div>
                <div class="price right">
                  <span>¥14.00</span>
                </div>
              </div>
              <footer class="clear">
                <span class="left">成都盛泓超纤皮革经营部</span>
                <span class="right">成都武侯</span>
              </footer>
            </div>
            <div class="mark">企业认证</div>
          </router-link>
          <router-link to="/detail" class="info-item" tag="li">
            <div class="icontent">
              <div class="title">水刺底仿猪皮革 无纺布底PU仿猪里皮</div>
              <div class="parameter">
                <div class="param-list left">
                  <div class="param-item">
                    <span class="value">黄牛皮</span>
                    <span class="param">品种</span>
                  </div>
                  <div class="param-item">
                    <span class="value">A级</span>
                    <span class="param">皮胚</span>
                  </div>
                  <div class="param-item">
                    <span class="value">0.7mm</span>
                    <span class="param">厚度</span>
                  </div>
                </div>
                <div class="price right">
                  <span>¥14.00</span>
                </div>
              </div>
              <footer class="clear">
                <span class="left">成都盛泓超纤皮革经营部</span>
                <span class="right">成都武侯</span>
              </footer>
            </div>
            <div class="mark">企业认证</div>
          </router-link>
          <router-link to="/detail" class="info-item" tag="li">
            <div class="icontent">
              <div class="title">水刺底仿猪皮革 无纺布底PU仿猪里皮</div>
              <div class="parameter">
                <div class="param-list left">
                  <div class="param-item">
                    <span class="value">黄牛皮</span>
                    <span class="param">品种</span>
                  </div>
                  <div class="param-item">
                    <span class="value">A级</span>
                    <span class="param">皮胚</span>
                  </div>
                  <div class="param-item">
                    <span class="value">0.7mm</span>
                    <span class="param">厚度</span>
                  </div>
                </div>
                <div class="price right">
                  <span>¥14.00</span>
                </div>
              </div>
              <footer class="clear">
                <span class="left">成都盛泓超纤皮革经营部</span>
                <span class="right">成都武侯</span>
              </footer>
            </div>
            <div class="mark">企业认证</div>
          </router-link>
          <router-link to="/detail" class="info-item" tag="li">
            <div class="icontent">
              <div class="title">水刺底仿猪皮革 无纺布底PU仿猪里皮</div>
              <div class="parameter">
                <div class="param-list left">
                  <div class="param-item">
                    <span class="value">黄牛皮</span>
                    <span class="param">品种</span>
                  </div>
                  <div class="param-item">
                    <span class="value">A级</span>
                    <span class="param">皮胚</span>
                  </div>
                  <div class="param-item">
                    <span class="value">0.7mm</span>
                    <span class="param">厚度</span>
                  </div>
                </div>
                <div class="price right">
                  <span>¥14.00</span>
                </div>
              </div>
              <footer class="clear">
                <span class="left">成都盛泓超纤皮革经营部</span>
                <span class="right">成都武侯</span>
              </footer>
            </div>
            <div class="mark">企业认证</div>
          </router-link>
          <li class="info-item">
            <div class="icontent">
              <div class="title">新款彩色平纹纳帕牛皮革</div>
              <div class="parameter">
                <div class="param-list left">
                  <div class="param-item">
                    <span class="value">黄牛皮</span>
                    <span class="param">品种</span>
                  </div>
                  <div class="param-item">
                    <span class="value">A级</span>
                    <span class="param">皮胚</span>
                  </div>
                  <div class="param-item">
                    <span class="value">1.2mm</span>
                    <span class="param">厚度</span>
                  </div>
                </div>
                <div class="price right">
                  <span>¥19.50</span>
                </div>
              </div>
              <footer class="clear">
                <span class="left">鼎茂皮革</span>
                <span class="right">广东 广州</span>
              </footer>
            </div>
            <!-- <div class="mark">企业认证</div> -->
          </li>
          <li class="load-more">加载更多</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import store from '@/utils/store.js'

export default {
  data () {
    return {
      user: {
        id: null,
        name: null,
        phone: null
      }
    }
  },
  created () {
    if (store.get('user') === null || !store.get('user', true).login) {
      this.$toast('请登录')
      setTimeout(() => {
        this.$router.push({path: '/login', query: { backhome: true }})
      }, 1500)
    } else {
      const userData = store.get('user', true)
      this.user.id = userData.uid
      this.user.name = userData.name
      this.user.phone = userData.phone
    }
  },
  methods: {
    goback () {
      this.$router.go(-1)
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../../../style/subpage';
@import '../../../style/infolist';

.user, .shop {
  overflow: auto;
}
.user-info {
  float: left;
  span {
    display: block;
  }
  .name {
    font-size: 4.2vw;
  }
  .phone {
    font-size: 3.8vw;
    color: $fontGray;
  }
}
.edit-button {
  margin-top: 1.6vw;
  padding: 1vw 2.6vw;
  display: inline-block;
  float: right;
  font-size: 3.6vw;
  color: #FF9650;
  background-color: #FFFBF2;
  border: 1px solid #FFE8D5;
  border-radius: 0.6vw;
}
.shop {
  padding: 3vw $wrap;
  border-top: 1px solid #ECEEF3;
  span {
    float: left;
    font-size: 3.8vw;
  }
  .iconfont {
    float: right;
    font-size: 5vw;
    color: #C5C9D2;
  }
}

.tab-container {
  background-color: #fff;
}
.tab {
  display: flex;
  border-bottom: 1px solid #E9EDF0;
  text-align: center;
}
.tab-item {
  margin: 0 17vw;
  padding: 2.8vw 0 1.8vw 0;
  flex: 1;
  font-size: 3.6vw;
  color: $fontGray;
  box-sizing: border-box;
}
.tab-active {
  color: #333;
  border-bottom: 0.6vw solid #FF7E5A;
}
.load-more {
  @include page-padding-bottom;
}

.slide-enter-active, .slide-leave-active {
  transition: .36s ease;
}
.slide-enter, .slide-leave-active {
  transform: translate(100%, 0);
}
</style>
