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
                            <td>trigger</td>
                            <td>触发方式</td>
                            <td>String</td>
                            <td>click/focus/hover/manual</td>
                            <td>click</td>
                        </tr>
                        <tr>
                            <td>title</td>
                            <td>标题</td>
                            <td>String</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>content</td>
                            <td>显示的内容，也可以通过 <code>slot</code> 传入 DOM</td>
                            <td>String</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>width</td>
                            <td>宽度</td>
                            <td>String, Number</td>
                            <td>—</td>
                            <td>最小宽度 150px</td>
                        </tr>
                        <tr>
                            <td>placement</td>
                            <td>出现位置</td>
                            <td>String</td>
                            <td>top/top-start/top-end/bottom/bottom-start/bottom-end/left/left-start/left-end/right/right-start/right-end</td>
                            <td>bottom</td>
                        </tr>
                        <tr>
                            <td>disabled</td>
                            <td>Popover 是否可用</td>
                            <td>Boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>value / v-model</td>
                            <td>状态是否可见</td>
                            <td>Boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>offset</td>
                            <td>出现位置的偏移量</td>
                            <td>Number</td>
                            <td>—</td>
                            <td>0</td>
                        </tr>
                        <tr>
                            <td>transition</td>
                            <td>定义渐变动画</td>
                            <td>String</td>
                            <td>—</td>
                            <td>fade-in-linear</td>
                        </tr>
                        <tr>
                            <td>visible-arrow</td>
                            <td>是否显示 Tooltip 箭头，更多参数可见<a href="https://github.com/element-component/vue-popper">Vue-popper</a></td>
                            <td>Boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>popper-options</td>
                            <td><a href="https://popper.js.org/documentation.html">popper.js</a> 的参数</td>
                            <td>Object</td>
                            <td>参考 <a href="https://popper.js.org/documentation.html">popper.js</a> 文档</td>
                            <td><code>{ boundariesElement: 'body', gpuAcceleration: false }</code></td>
                        </tr>
                        <tr>
                            <td>popper-class</td>
                            <td>为 popper 添加类名</td>
                            <td>String</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>open-delay</td>
                            <td>触发方式为 hover 时的显示延迟，单位为毫秒</td>
                            <td>Number</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>close-delay</td>
                            <td>触发方式为 hover 时的隐藏延迟，单位为毫秒</td>
                            <td>number</td>
                            <td>—</td>
                            <td>200</td>
                        </tr>
                        <tr>
                            <td>tabindex</td>
                            <td>Popover 组件的 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex">tabindex</a></td>
                            <td>number</td>
                            <td>—</td>
                            <td>0</td>
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
                            <th>参数</th>
                            <th>说明</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>—</td>
                            <td>Popover 内嵌 HTML 文本</td>
                        </tr>
                        <tr>
                            <td>reference</td>
                            <td>触发 Popover 显示的 HTML 元素</td>
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
                            <td>show</td>
                            <td>显示时触发</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>after-enter</td>
                            <td>显示动画播放完毕后触发</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>hide</td>
                            <td>隐藏时触发</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>after-leave</td>
                            <td>隐藏动画播放完毕后触发</td>
                            <td>—</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
    </div>
</template>


