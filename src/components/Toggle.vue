<template>
    <label class="label-switch switch-primary my-0">
        <input type="checkbox" class="switch switch-bootstrap status" name="status" id="status" value="1" checked="checked">
        <span class="lable"></span>
    </label>
</template>

<script>
export default {
  name: "Toggle"
};
</script>

<style scoped>
.switch {
  opacity: 0;
  position: absolute;
  z-index: 1;
  width: 18px;
  height: 18px;
  cursor: pointer;
}

.switch + .lable {
  position: relative;
  display: inline-block;
  margin: 0;
  line-height: 20px;
  min-height: 18px;
  min-width: 18px;
  font-weight: normal;
  cursor: pointer;
}

.switch + .lable::before {
  cursor: pointer;
  font-weight: normal;
  font-size: 12px;
  color: #32a3ce;
  background-color: #fafafa;
  border: 1px solid #c8c8c8;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
  border-radius: 0;
  display: inline-block;
  text-align: center;
  height: 16px;
  line-height: 14px;
  min-width: 16px;
  margin-right: 1px;
  position: relative;
  top: -1px;
}

.switch:checked + .lable::before {
  display: inline-block;
  content: "\f00c";
  background-color: #f5f8fc;
  border-color: #adb8c0;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05),
    inset 0px -15px 10px -12px rgba(0, 0, 0, 0.05),
    inset 15px 10px -12px rgba(255, 255, 255, 0.1);
}

.switch + .lable::before {
  font-weight: normal;
  font-size: 11px;
  line-height: 17px;
  height: 20px;
  overflow: hidden;
  border-radius: 12px;
  background-color: #f5f5f5;
  -webkit-box-shadow: inset 0 1px 1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 1px 1px 0 rgba(0, 0, 0, 0.15);
  border: 1px solid #ccc;
  text-align: left;
  float: left;
  padding: 0;
  width: 52px;
  text-indent: -21px;
  margin-right: 0;
  -webkit-transition: text-indent 0.3s ease;
  -o-transition: text-indent 0.3s ease;
  transition: text-indent 0.3s ease;
  top: auto;
}

.switch.switch-bootstrap + .lable::before {
  content: "";
  box-shadow: none;
  border-width: 0;
  font-size: 16px;
  background-color: #a9a9a9;
  color: #f2f2f2;
  width: 52px;
  height: 22px;
  line-height: 21px;
  text-indent: 32px;
  -webkit-transition: background 0.1s ease;
  -o-transition: background 0.1s ease;
  transition: background 0.1s ease;
}

.switch.switch-bootstrap + .lable::after {
  content: "";
  position: absolute;
  top: 2px;
  left: 3px;
  border-radius: 12px;
  box-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
  width: 18px;
  height: 18px;
  text-align: center;
  background-color: #f2f2f2;
  border: 4px solid #f2f2f2;
  -webkit-transition: left 0.2s ease;
  -o-transition: left 0.2s ease;
  transition: left 0.2s ease;
}

.switch.switch-bootstrap:checked + .lable::before {
  text-indent: 6px;
  color: #fff;
  border-color: #b7d3e5;
}

.switch-primary > .switch.switch-bootstrap:checked + .lable::before {
  background-color: #0d1532;
}

.switch.switch-bootstrap:checked + .lable::after {
  left: 32px;
  background-color: #fff;
  border: 4px solid #fff;
  text-shadow: 0 -1px 0 rgba(0, 200, 0, 0.25);
}

/* square */
.switch-square {
  opacity: 0;
  position: absolute;
  z-index: 1;
  width: 18px;
  height: 18px;
  cursor: pointer;
}

.switch-square + .lable {
  position: relative;
  display: inline-block;
  margin: 0;
  line-height: 20px;
  min-height: 18px;
  min-width: 18px;
  font-weight: normal;
  cursor: pointer;
}

.switch-square + .lable::before {
  cursor: pointer;
  font-weight: normal;
  font-size: 12px;
  color: #32a3ce;
  background-color: #fafafa;
  border: 1px solid #c8c8c8;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
  border-radius: 0;
  display: inline-block;
  text-align: center;
  height: 16px;
  line-height: 14px;
  min-width: 16px;
  margin-right: 1px;
  position: relative;
  top: -1px;
}

.switch-square:checked + .lable::before {
  display: inline-block;
  background-color: #f5f8fc;
  border-color: #adb8c0;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05),
    inset 0px -15px 10px -12px rgba(0, 0, 0, 0.05),
    inset 15px 10px -12px rgba(255, 255, 255, 0.1);
}

/* CSS3 on/off switches */
.switch-square + .lable {
  margin: 0 4px;
  min-height: 24px;
}

.switch-square + .lable::before {
  font-weight: normal;
  font-size: 11px;
  line-height: 17px;
  height: 20px;
  overflow: hidden;
  border-radius: 2px;
  background-color: #f5f5f5;
  -webkit-box-shadow: inset 0 1px 1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 1px 1px 0 rgba(0, 0, 0, 0.15);
  border: 1px solid #ccc;
  text-align: left;
  float: left;
  padding: 0;
  width: 52px;
  text-indent: -21px;
  margin-right: 0;
  -webkit-transition: text-indent 0.3s ease;
  -o-transition: text-indent 0.3s ease;
  transition: text-indent 0.3s ease;
  top: auto;
}

.switch-square.switch-bootstrap + .lable::before {
  box-shadow: none;
  border-width: 0;
  font-size: 16px;
  background-color: #a9a9a9;
  color: #f2f2f2;
  width: 52px;
  height: 22px;
  line-height: 21px;
  text-indent: 32px;
  -webkit-transition: background 0.1s ease;
  -o-transition: background 0.1s ease;
  transition: background 0.1s ease;
}

.switch-square.switch-bootstrap + .lable::after {
  content: "";
  position: absolute;
  top: 2px;
  left: 3px;
  border-radius: 12px;
  box-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
  width: 18px;
  height: 18px;
  text-align: center;
  background-color: #f2f2f2;
  border: 4px solid #f2f2f2;
  -webkit-transition: left 0.2s ease;
  -o-transition: left 0.2s ease;
  transition: left 0.2s ease;
}

.switch-square.switch-bootstrap:checked + .lable::before {
  content: "\f00c";
  text-indent: 6px;
  color: #fff;
  border-color: #b7d3e5;
}

.switch-primary > .switch-square.switch-bootstrap:checked + .lable::before {
  background-color: #337ab7;
}

.switch-square.switch-bootstrap:checked + .lable::after {
  left: 32px;
  background-color: #fff;
  border: 4px solid #fff;
  text-shadow: 0 -1px 0 rgba(0, 200, 0, 0.25);
}

.switch-square.switch-bootstrap + .lable::after {
  border-radius: 2px;
}
</style>