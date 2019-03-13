<template>
  <div class="activity layout">
    <dl class="activityList">
      <dt class="first">
        <a href="">
          <div class="title">
            <em class="redC">限时抢购</em>
            <ul class="downTime">
              <li><span>00</span> </li>
              <li><span>00</span></li>
              <li><span>00</span></li>
            </ul>
          </div>
        </a>
      </dt>
      <dd>
        <a href="">
          <div class="title">
            <em class="orgC">每日开团</em>
          </div>
        </a>
      </dd>
      <dd>
        <a href="">
          <div class="title"><em class="yelC">砍价实惠</em></div>
        </a>
      </dd>
      <dd>
        <a href="">
          <div class="title"><em class="bluC">精品课程</em></div>
        </a>
      </dd>
    </dl>
    <ul class="courseList">
      <li><a href=""><em>人工智能物联网</em></a></li>
      <li><a href=""><em>人工智能Python</em></a></li>
      <li><a href=""><em>大数据开发/分析</em></a></li>
      <li><a href=""><em>JavaEE全栈开发</em></a></li>
      <li><a href=""><em>Web前端+H5开发</em></a></li>
    </ul>
  </div>
</template>

<script type='text/ecmascript-6'>
export default {

}
</script>

<style scoped lang='less'>
@redC: #fb2029;
@orgC: #ff6000;
@yelC: #f8ba0b;
@bluC: #039bfb;
@whiC: #fff;
@dadC: #dadada;
.redC {
  color: @redC;
}
.orgC {
  color: @orgC;
}
.yelC {
  color: @yelC;
}
.bluC {
  color: @bluC;
}
.borderBox {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
  .activity {
    height: 5.72rem;
    background: @whiC;
    dl {
      width: 7.5rem;
      height: 3.8rem;
      overflow: hidden;
      border-bottom: 1px solid @dadC;
      .borderBox;
      .first {
        height: 1.9rem;
        width: 3.75rem;
        border-right: 1px solid @dadC;
        float: left;
        overflow: hidden;
        padding: 0.3rem 0.2rem;
        .borderBox;
        .title {
          font-size: 0.28rem;
          ul {
            float: right;
            li {
              float: left;
              color: @whiC;
              font-size: 0.24rem;
              span {
                display: inline-block;
                width: 0.34rem;
                height: 0.3rem;
                background-color: #000000;
                text-align: center;
                border-radius: 0.05rem;
                line-height: 0.3rem;
              }
            }
            li::after {
              content: ':';
              color: #000000;
              margin: 0.07rem;
            }
            li:last-child::after {
              content: '';
              margin: 0;
            }
          }
        }
        a {
          display: inline-block;
          width: 100%;
          height: 100%;
        }
      }
      dd {
        .first;
        border-right: none;
      }
      dd:nth-child(3) {
        border-right: 1px solid @dadC;
      }
      dd+dd {
        border-top: 1px solid @dadC;
      }
    }
    .courseList {
      height: 1.9rem;
      width: 7.5rem;
      display: flex;
      display: -webkit-flex;
      li {
        height: 1.9rem;
        flex: 1;
        padding: 0.2rem;
        .borderBox;
        color: #333333;
        a {
          color: inherit;
        }
      }
      li + li {
        border-left: 1px solid @dadC;
      }
    }
  }
</style>
