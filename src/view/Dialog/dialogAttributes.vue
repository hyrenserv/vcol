<template>
    <div>
        <el-collapse>
            <el-collapse-item title="属性" name="1">
                <table>
                    <thead>
                        <tr>
                            <th>参数</th>
                            <th>说明</th>
                            <th>类型</th>
                            <th>可选值</th>
                            <th>默认值</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>visible</td>
                            <td>是否显示 Dialog，支持 .sync 修饰符</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>title</td>
                            <td>Dialog 的标题，也可通过具名 slot （见下表）传入</td>
                            <td>string</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>width</td>
                            <td>Dialog 的宽度</td>
                            <td>string</td>
                            <td>—</td>
                            <td>50%</td>
                        </tr>
                        <tr>
                            <td>fullscreen</td>
                            <td>是否为全屏 Dialog</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>top</td>
                            <td>Dialog CSS 中的 margin-top 值</td>
                            <td>string</td>
                            <td>—</td>
                            <td>15vh</td>
                        </tr>
                        <tr>
                            <td>modal</td>
                            <td>是否需要遮罩层</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>modal-append-to-body</td>
                            <td>遮罩层是否插入至 body 元素上，若为 false，则遮罩层会插入至 Dialog 的父元素上</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>append-to-body</td>
                            <td>Dialog 自身是否插入至 body 元素上。嵌套的 Dialog 必须指定该属性并赋值为 true</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>lock-scroll</td>
                            <td>是否在 Dialog 出现时将 body 滚动锁定</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>custom-class</td>
                            <td>Dialog 的自定义类名</td>
                            <td>string</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>close-on-click-modal</td>
                            <td>是否可以通过点击 modal 关闭 Dialog</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>close-on-press-escape</td>
                            <td>是否可以通过按下 ESC 关闭 Dialog</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>show-close</td>
                            <td>是否显示关闭按钮</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>before-close</td>
                            <td>关闭前的回调，会暂停 Dialog 的关闭</td>
                            <td>function(done)，done 用于关闭 Dialog</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>center</td>
                            <td>是否对头部和底部采用居中布局</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>destroy-on-close</td>
                            <td>关闭时销毁 Dialog 中的元素</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
        
        <el-collapse>
            <el-collapse-item title="Slot" name="1">
                <table>
                    <thead>
                        <tr>
                            <th>name</th>
                            <th>说明</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>—</td>
                            <td>Dialog 的内容</td>
                        </tr>
                        <tr>
                            <td>title</td>
                            <td>Dialog 标题区的内容</td>
                        </tr>
                        <tr>
                            <td>footer</td>
                            <td>Dialog 按钮操作区的内容</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
        
        <el-collapse>
            <el-collapse-item title="事件" name="1">
                <table>
                    <thead>
                        <tr>
                            <th>事件名称</th>
                            <th>说明</th>
                            <th>回调参数</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>open</td>
                            <td>Dialog 打开的回调</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>opened</td>
                            <td>Dialog 打开动画结束时的回调</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>close</td>
                            <td>Dialog 关闭的回调</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>closed</td>
                            <td>Dialog 关闭动画结束时的回调</td>
                            <td>—</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
    </div>
</template>
