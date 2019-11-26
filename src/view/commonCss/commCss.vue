<template>
<div class="common">
    <h3> 直接更改样式如若未生效，自行添加<span>!important</span></h3>
    <h4>button class</h4>
    /* 按钮设置样式的class名称,需要给button设置class="elButton"实现更改样式*/</br>
    /*按钮大小设置需在el-button标签设置size属性实现*/</br>
    /*删除 确定 取消 可以通过设置button的type属性实现*/</br>
    .elButton {}</br>
    <h5>button的type</h5>
    <h5>(1)primary</h5>
    .el-button--primary {
    color: #FFF !important;
    background-color: #3a8ee6 !important;
    border-color: #3a8ee6 !important;
    }</br>

    <h5>(2)success</h5>
    .el-button--success {
    color: #FFF;
    background-color: #67C23A;
    border-color: #67C23A
    }</br>

    <h5>(3)warning</h5>
    .el-button--warning {
    color: #FFF;
    background-color: #E6A23C;
    border-color: #E6A23C
    }</br>

    <h5>(4)danger</h5>
    .el-button--danger {
    color: #FFF;
    background-color: #F56C6C;
    border-color: #F56C6C
    }</br>

    <h5>(5)info</h5>
    .el-button--info {
    color: #FFF;
    background-color: #909399;
    border-color: #909399
    }</br>

    <h4>table class</h4>

    /* 表格表头样式,不需要添加属性即可更改，如有特别样式请自行设置class名谢谢 */</br>
    .el-table th {
    background-color: #3d8dd2 !important;
    color: #fff;
    height: 20px !important;
    line-height: 20px !important;
    }</br>

    /* 斑马纹样式，需要在table里面写stripe属性然后在这里实现样式的更改 */</br>
    .el-table--striped .el-table__body tr.el-table__row--striped td {
    background-color: rgb(252, 249, 249) !important;
    }</br>

    /* 表格td样式，不需要添加属性即可更改 */</br>
    .el-table--enable-row-transition .el-table__body td {
    /* background-color: cyan; */
    }</br>

    /* 其他表格鼠标划入时的颜色，不需要添加属性即可更改 */</br>
    .el-table--enable-row-hover .el-table__body tr:hover>td {
    /* background-color:#7ba6cf86 !important; */
    }</br>

    /* 默认表格鼠标划入时的颜色，不需要添加属性即可更改 */</br>
    .el-table__body tr.hover-row.current-row>td,
    .el-table__body tr.hover-row.el-table__row--striped.current-row>td,
    .el-table__body tr.hover-row.el-table__row--striped>td,
    .el-table__body tr.hover-row>td {
    /* background-color:#7ba6cf86 !important; */
    }</br>

    <h4>radio class</h4>

    /*单选框默认样式设置，不需要添加属性，可以直接更改*/ </br>
    .el-radio__inner {}</br>

    /*单选框默认字体样式设置，不需要添加属性，可以直接更改*/
    .el-radio__label {}</br>

    /*单选框选中样式设置，不需要添加属性，可以直接更改*/</br>
    .el-radio__input.is-checked .el-radio__inner {}</br>

    /*单选框选中字体样式设置，不需要添加属性，可以直接更改*/</br>
    .el-radio__input.is-checked+.el-radio__label {}</br>

    /* 如果需要只设置单独的某一个radio，需要在el-radio添加id="manuallyChange"实现 */</br>
    /*单选框样式设置*/</br>
    #manuallyChange .el-radio__inner {}</br>

    /*单选框字体样式设置，*/</br>
    #manuallyChange .el-radio__label {}</br>

    /*单选框选中样式设置*/</br>
    #manuallyChange .el-radio__input.is-checked .el-radio__inner {
    /* border-color:rgb(83, 168, 33);
    background: rgb(83, 168, 33); */
    }</br>

    /*单选框选中字体样式设置*/</br>
    #manuallyChange .el-radio__input.is-checked+.el-radio__label {
    /* color: rgb(83, 168, 33); */
    }</br>

    <h4>message class</h4>
    /* 在更改样式之前，需要在methods的方法this.$confirm里添加cancelButtonClass或者confirmButtonClass */</br>
    /*message取消按钮的默认样式*/</br>
    .btn-cancel {
    background-color: #F56C6C;
    color: #FFFFFF;
    border: 1px solid #F56C6C;
    }</br>

    .btn-cancel:hover {
    background-color: #F56C6C;
    color: #FFFFFF;
    border: 1px solid #F56C6C;
    }</br>

    /*message确认按钮的默认样式*/</br>
    .btn-confirm {}</br>

    /* */

    <h4>input class</h4>

    /*input表单验证提示信息样式，不需要添加属性，可以直接更改*/</br>
    .el-form-item__error {}</br>

    /*input表单验证提示信息样式边框，不需要添加属性，可以直接更改*/</br>
    .el-form-item.is-error .el-input__inner,
    .el-form-item.is-error .el-textarea__inner {
    /* border-color: blue; */
    }</br>
    /* 被禁用时候的样式更改 */</br>
    .el-input.is-disabled .el-input__inner {
    /* background-color: blue;
    border-color: #E4E7ED;
    color: #C0C4CC;
    cursor: not-allowed; */
    }</br>

    <h4>checkbox class</h4>

    /*复选框默认样式设置，不需要添加属性，可以直接更改*/</br>
    .el-checkbox__inner {}</br>

    /*复选框默认字体样式设置，不需要添加属性，可以直接更改*/</br>
    .el-checkbox__label {}</br>

    /*复选框默认选中样式设置，不需要添加属性，可以直接更改*/</br>
    .el-checkbox__input.is-checked .el-checkbox__inner {}</br>

    /*复选框字体默认选中样式设置，不需要添加属性，可以直接更改*/</br>
    .el-checkbox__input.is-checked+.el-checkbox__label {}</br>

    /* 如果需要只设置单独的某一个复选框，需要在el-checkbox添加id="manuallyChangeck"实现 */</br>
    /*复选框样式设置*/</br>
    #manuallyChangeck .el-checkbox__inner {}</br>

    /*复选框字体样式设置*/</br>
    #manuallyChangeck .el-checkbox__label {}</br>

    /*复选框选中样式设置*/</br>
    #manuallyChangeck .el-checkbox__input.is-checked .el-checkbox__inner {}</br>

    /*复选框选中字体设置*/</br>
    #manuallyChangeck .el-checkbox__input.is-checked+.el-checkbox__label {}</br>

    <h4>tab选项卡 class</h4>
    /*选项卡的默认样式*/</br>
    .el-tabs__nav-scroll {
    background: #95b6f330;
    }</br>

    /*选项卡的选中默认样式*/</br>
    .el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active {
    /* background-color: chartreuse;
    color: coral; */
    }</br>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.common {
    text-align: left;
}

h3 {
    text-align: center;
}
span{
    color: blue;
}
</style>
