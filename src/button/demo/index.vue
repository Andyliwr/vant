<template>
  <demo-section>
    <demo-block :title="$t('type')">
      <div class="demo-button-row">
        <van-button type="default">{{ $t('default') }}</van-button>
        <van-button type="primary">{{ $t('primary') }}</van-button>
        <van-button type="info">{{ $t('info') }}</van-button>
      </div>
      <van-button type="danger">{{ $t('danger') }}</van-button>
      <van-button type="warning">{{ $t('warning') }}</van-button>
    </demo-block>

    <demo-block :title="$t('plain')">
      <van-button
        plain
        type="primary"
        :text="$t('plain')"
      />
      <van-button
        plain
        type="danger"
        :text="$t('plain')"
      />
    </demo-block>

    <demo-block :title="$t('hairline')">
      <van-button
        plain
        hairline
        type="primary"
        :text="$t('hairlineButton')"
      />
      <van-button
        plain
        hairline
        type="danger"
        :text="$t('hairlineButton')"
      />
    </demo-block>

    <demo-block :title="$t('disabled')">
      <van-button
        disabled
        type="primary"
        :text="$t('disabled')"
      />
      <van-button
        disabled
        type="danger"
        :text="$t('disabled')"
      />
    </demo-block>

    <demo-block :title="$t('loadingStatus')">
      <van-button
        loading
        type="primary"
      />
      <van-button
        loading
        type="primary"
        loading-type="spinner"
      />
      <van-button
        loading
        :loading-text="$t('loadingText')"
        type="danger"
      />
    </demo-block>

    <demo-block :title="$t('shape')">
      <van-button
        type="primary"
        square
        :text="$t('square')"
      />
      <van-button
        type="danger"
        round
        :text="$t('round')"
      />
    </demo-block>

    <demo-block :title="$t('icon')">
      <van-button
        type="primary"
        icon="star-o"
      />
      <van-button
        type="primary"
        icon="star-o"
        :text="$t('button')"
      />
      <van-button
        plain
        type="primary"
        icon="https://img.yzcdn.cn/vant/logo.png"
        :text="$t('button')"
      />
    </demo-block>

    <demo-block :title="$t('size')">
      <van-button
        type="primary"
        size="large"
      >
        {{ $t('large') }}
      </van-button>
      <van-button
        type="primary"
        size="normal"
      >
        {{ $t('normal') }}
      </van-button>
      <van-button
        type="primary"
        size="small"
      >
        {{ $t('small') }}
      </van-button>
      <van-button
        type="primary"
        size="mini"
      >
        {{ $t('mini') }}
      </van-button>
    </demo-block>

    <demo-block :title="$t('router')">
      <van-button
        :text="$t('urlRoute')"
        type="primary"
        url="/vant/mobile.html"
      />
      <van-button
        :text="$t('vueRoute')"
        type="primary"
        to="index"
      />
    </demo-block>

    <demo-block :title="$t('customColor')">
      <van-button
        color="#7232dd"
        :text="$t('customColor')"
      />
      <van-button
        plain
        color="#7232dd"
        :text="$t('customColor')"
      />
    </demo-block>
  </demo-section>
</template>

<script>
export default {
  i18n: {
    'zh-CN': {
      type: '按钮类型',
      size: '按钮尺寸',
      icon: '图标按钮',
      loading: '加载状态',
      shape: '按钮形状',
      default: '默认按钮',
      primary: '主要按钮',
      info: '信息按钮',
      danger: '危险按钮',
      warning: '警告按钮',
      large: '大号按钮',
      normal: '普通按钮',
      small: '小型按钮',
      mini: '迷你按钮',
      plain: '朴素按钮',
      square: '方形按钮',
      round: '圆形按钮',
      hairline: '细边框',
      hairlineButton: '细边框按钮',
      loadingText: '加载中...',
      router: '页面导航',
      urlRoute: 'URL 跳转',
      vueRoute: '路由跳转',
      customColor: '自定义颜色'
    },
    'en-US': {
      type: 'Type',
      size: 'Size',
      icon: 'Icon',
      loading: 'Loading',
      shape: 'Shape',
      default: 'Default',
      primary: 'Primary',
      info: 'Info',
      danger: 'Danger',
      warning: 'Warning',
      large: 'Large',
      normal: 'Normal',
      small: 'Small',
      mini: 'Mini',
      plain: 'Plain',
      square: 'Square',
      round: 'Round',
      hairline: 'Hairline',
      hairlineButton: 'Hairline',
      loadingText: 'Loading...',
      router: 'Router',
      urlRoute: 'URL',
      vueRoute: 'Vue Router',
      customColor: 'Custom Color'
    }
  }
};
</script>

<style lang="less">
@import "../../style/var";

.demo-button {
  .van-button {
    &--large {
      margin-bottom: @padding-md;
    }

    &--small,
    &--normal:not(:last-child) {
      margin-right: @padding-md;
    }
  }

  .van-doc-demo-block {
    padding: 0 @padding-md;
  }

  .van-doc-demo-block__title {
    padding-left: 0;
  }

  &-row {
    margin-bottom: @padding-sm;
  }
}
</style>
