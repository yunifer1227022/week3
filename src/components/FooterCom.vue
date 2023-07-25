<template>
  <div class="footer">
    <div class="container flex jcsb ai-center footer-navbar">
      <div class="footer-nav">
        <ul class="flex">
          <li><a href="#">首頁</a></li>
          <li><a href="#">系列鏡架</a></li>
          <li><a href="#">門市據點</a></li>
          <li><a href="#">部落格</a></li>
          <li><a href="#">常見問題</a></li>
        </ul>
      </div>
      <div class="footer-icon">
        <a href="#"
          ><img
            src="https://github.com/hexschool/2022-web-layout-training/blob/main/week3-4/ic-social-fb.png?raw=true"
            alt="facebook"
        /></a>
        <a href="#"
          ><img
            src="https://github.com/hexschool/2022-web-layout-training/blob/main/week3-4/ic_social_ig.png?raw=true"
            alt="ig"
        /></a>
        <a href="#"
          ><img
            src="https://github.com/hexschool/2022-web-layout-training/blob/main/week3-4/ic_social_line.png?raw=true"
            alt="line"
        /></a>
      </div>
    </div>
    <!-- contact -->
    <div class="footer-contact container">
      <div class="footer-contact-section">
        <a class="" href="tel:0800000000"
          ><i class="bi bi-telephone"></i><span>0800-000-000</span></a
        >
      </div>
      <div class="footer-contact-section border-bottom">
        <a class="" href="mailto:glasses@business.com"
          ><i class="bi bi-envelope"></i><span>glasses@business.com</span></a
        >
      </div>
      <!-- copyright -->
      <div class="copyright flex jcsb ai-center">
        <div class="copyright-section">
          <p>Copyright © 2020 Glasses.All rights reserved.</p>
        </div>
        <div class="copyright-clause flex">
          <a href="#" class="fz-14">隱私權政策</a>
          <a href="#" class="fz-14">服務條款</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@import '../assets/base.scss';
@import url('https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css');
.footer {
  background: $primary;
  padding-top: 32px;
  @include mobile {
    display: flex;
    flex-direction: row-reverse;
    align-items: flex-start;
    position: relative;
  }
  &-navbar {
    margin-bottom: 36px;
    @include pad {
      margin-bottom: 30px;
    }
    .footer-nav {
      @include mobile {
        display: none;
      }
      a {
        color: $white;
        vertical-align: middle;
        margin-right: 48px;
      }
    }
    .footer-icon {
      vertical-align: middle;
      @include mobile {
        position: absolute;
        right: 14px;
      }
      img {
        width: 48px;
        height: 48px;
        margin-left: 32px;
        @include pad {
          width: 40px;
          height: 40px;
          margin-left: 16px;
        }
        @include mobile {
          width: 24px;
          height: 24px;
        }
      }
    }
  }
  &-contact {
    @include mobile {
      order: 1;
    }
    align-items: flex-start;
    .border-bottom {
      border-bottom: 1px solid #fff;
      padding-bottom: 32px;
    }
    &-section {
      margin-bottom: 0px;
      &:first-child {
        margin-bottom: 8px;
      }
      @include mobile {
        width: 100%;
      }
      a {
        color: $white;
        font-size: 36px;
        @include mobile {
          font-size: 16px;
        }
        i {
          width: 36px;
          height: 36px;
          margin-right: 20px;
          @include mobile {
            margin-right: 11px;
          }
        }
      }
    }
    .copyright {
      @include mobile {
        flex-direction: column;
        align-items: flex-start;
      }
      &-section {
        color: $white;
        padding: 32px 0px 40px 0px;
        @include mobile {
          padding: 16px 0px 8px 0px;
        }
      }
      &-clause {
        @include mobile {
          flex-direction: column;
        }
        margin: 32px 0;
        @include mobile {
          margin: 0px 0px 24px 0px;
        }
        a {
          margin-left: 48px;
          color: $white;
          @include mobile {
            margin: 8px 0px;
          }
        }
      }
    }
  }
}
</style>
