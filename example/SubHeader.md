## SubHeader

SubHeader 组件用于描述和区分列表（或网格列表）中不同的区块，通常与当前筛选和排序准则相关联。

#### 示例

配合列表使用

```san Simple Usage with List
<template>
  <div class="sm-list-wrapper">
      <san-list>
          <san-sub-header>最近聊天记录</san-sub-header>
          <san-list-item primaryText="Junmer">
              <san-avatar slot="left" src="http://boscdn.bpc.baidu.com/movie/assets/avatar1.jpeg"/>
              <san-icon slot="right">chat_bubble</san-icon>
          </san-list-item>
          <san-list-item primaryText="Leon Lu">
              <san-avatar slot="left" src="http://boscdn.bpc.baidu.com/movie/assets/avatar1.jpeg"/>
              <san-icon slot="right">chat_bubble</san-icon>
          </san-list-item>
          <san-list-item primaryText="Zhiqiang Zhang">
              <san-avatar slot="left" src="http://boscdn.bpc.baidu.com/movie/assets/avatar1.jpeg"/>
              <san-icon slot="right">chat_bubble</san-icon>
          </san-list-item>
          <san-list-item primaryText="CK Yaw">
              <san-avatar slot="left" src="http://boscdn.bpc.baidu.com/movie/assets/avatar1.jpeg"/>
              <san-icon slot="right">chat_bubble</san-icon>
          </san-list-item>
      </san-list>
      <san-divider />
      <san-list>
          <san-sub-header>历史聊天记录</san-sub-header>
          <san-list-item primaryText="Huiquan Huang">
              <san-avatar slot="left" src="http://boscdn.bpc.baidu.com/movie/assets/avatar1.jpeg"/>
              <san-icon slot="right">chat_bubble</san-icon>
          </san-list-item>
      </san-list>
  </div>
</template>
<script>
import Icon from '../src/Icon';
import SubHeader from '../src/SubHeader';
import {List, ListItem} from '../src/List';
import Avatar from '../src/Avatar';
import Divider from '../src/Divider';
import '../src/Avatar/Avatar.styl';
import '../src/SubHeader/SubHeader.styl';
import '../src/List/index.styl';
import '../src/Divider/Divider.styl';
export default {
    components: {
        'san-sub-header': SubHeader,
        'san-icon': Icon,
        'san-list': List,
        'san-list-item': ListItem,
        'san-divider': Divider,
        'san-avatar': Avatar
    }
};
</script>
<style>
.sm-list-wrapper {
    border: 1px solid #e1e1e1;
    max-width: 360px;
}
</style>
```

向内缩进示例

```san inset SubHeader
<template>
  <div class="sm-list-wrapper">
      <san-list>
          <san-sub-header inset="{{!0}}">Folders</san-sub-header>
          <san-list-item primaryText="Photos">
              <san-avatar slot="left" icon="folder"/>
              <san-icon slot="right">info</san-icon>
          </san-list-item>
          <san-list-item primaryText="Recipes">
              <san-avatar slot="left" icon="folder"/>
              <san-icon slot="right">info</san-icon>
          </san-list-item>
          <san-list-item primaryText="Work">
              <san-avatar slot="left" icon="folder"/>
              <san-icon slot="right">info</san-icon>
          </san-list-item>
      </san-list>
  </div>
</template>
<script>
import Icon from '../src/Icon';
import SubHeader from '../src/SubHeader';
import {List, ListItem} from '../src/List';
import Avatar from '../src/Avatar';
import Divider from '../src/Divider';
import '../src/Avatar/Avatar.styl';
import '../src/SubHeader/SubHeader.styl';
import '../src/List/index.styl';
import '../src/Divider/Divider.styl';
export default {
    components: {
        'san-sub-header': SubHeader,
        'san-icon': Icon,
        'san-list': List,
        'san-list-item': ListItem,
        'san-divider': Divider,
        'san-avatar': Avatar
    }
};
</script>
<style>
.sm-list-wrapper {
    border: 1px solid #e1e1e1;
    max-width: 360px;
}
</style>
```