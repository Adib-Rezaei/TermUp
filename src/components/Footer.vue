<template>
  <div id="footer">
    <p class="copyright">
      <i class="mdi mdi-copyright"></i>{{ copyright.farsiNum() }} | توسعه داده شده از روی بیکاری توسط<a href="https://t.me/danamirafzal" target="_blank">danamirafzal@.</a>
    </p>
    <div class="links">
      <a :href="repoUrl" target="_blank">
        <i class="mdi mdi-open-in-new"></i>
        مخزن پروژه
      </a>
      <router-link to="/contributors">
        <!-- <i class="mdi mdi-account-multiple"></i> -->
        مشارکت کنندگان
      </router-link>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
  data: function () {
    return {
      copyright: "کپی رایت 2022",
      repoUrl: "https://github.com/danamira/TermUp",
    };
  },
};
</script>
<style>
#footer {
  padding: 10px 20px;
  overflow: hidden;
  min-width: 1230px;
  width: 100%;
  margin-top: 30px;
  flex: none;
}
#footer .copyright {
  color: #293240;
  display: block;
  float: right;
  line-height: 24px;
  font-size: 14px;
}
#footer .copyright .mdi-copyright {
  display: block;
  float: right;
  line-height: 23px;
  font-size: 20px;
  margin-left: 6px;
}
#footer .copyright a {
    /* border: 1px solid  ; */
    cursor: pointer;
    font-size: 14px;
    color: rgb(85, 95, 112);
    padding: 1px 6px;
    border-radius: 4px;
    direction: ltr !important;
    text-align: left;
}
.links {
  float: left;
}
.links a {
  display: block;
  float: left;
  padding: 0 10px;
  color: #334052;
  line-height: 20px;
  height: 20px;
  text-decoration: none;
  font-size: 14px;
  border-right: 1px solid #b9c3c7;
}
.links a:last-child {
  border-right: none;
}
.links a .mdi {
  font-size: 19px;
  color: #7f899b;
  float: right;
  display: block;
  margin-left: 4px;
  line-height: 18px;
}
</style>