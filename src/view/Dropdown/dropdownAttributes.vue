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
                            <td>type</td>
                            <td>菜单按钮类型，同 Button 组件(只在<code>split-button</code>为 true 的情况下有效)</td>
                            <td>string</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>size</td>
                            <td>菜单尺寸，在<code>split-button</code>为 true 的情况下也对触发按钮生效</td>
                            <td>string</td>
                            <td>medium / small / mini</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>split-button</td>
                            <td>下拉触发元素呈现为按钮组</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>placement</td>
                            <td>菜单弹出位置</td>
                            <td>string</td>
                            <td>top/top-start/top-end/bottom/bottom-start/bottom-end</td>
                            <td>bottom-end</td>
                        </tr>
                        <tr>
                            <td>trigger</td>
                            <td>触发下拉的行为</td>
                            <td>string</td>
                            <td>hover, click</td>
                            <td>hover</td>
                        </tr>
                        <tr>
                            <td>hide-on-click</td>
                            <td>是否在点击菜单项后隐藏菜单</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>true</td>
                        </tr>
                        <tr>
                            <td>show-timeout</td>
                            <td>展开下拉菜单的延时（仅在 trigger 为 hover 时有效）</td>
                            <td>number</td>
                            <td>—</td>
                            <td>250</td>
                        </tr>
                        <tr>
                            <td>hide-timeout</td>
                            <td>收起下拉菜单的延时（仅在 trigger 为 hover 时有效）</td>
                            <td>number</td>
                            <td>—</td>
                            <td>150</td>
                        </tr>
                        <tr>
                            <td>tabindex</td>
                            <td>Dropdown 组件的 <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex">tabindex</a></td>
                            <td>number</td>
                            <td>—</td>
                            <td>0</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>

        <el-collapse>
            <el-collapse-item title="Slots" name="1">
                <table>
                    <thead>
                        <tr>
                            <th>Name</th>
                            <th>说明</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>—</td>
                            <td>触发下拉列表显示的元素。 注意： 必须是一个元素或者或者组件</td>
                        </tr>
                        <tr>
                            <td>dropdown</td>
                            <td>下拉列表，通常是 <code>&lt;el-dropdown-menu&gt;</code> 组件</td>
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
                            <td>click</td>
                            <td><code>split-button</code> 为 true 时，点击左侧按钮的回调</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>command</td>
                            <td>点击菜单项触发的事件回调</td>
                            <td>dropdown-item 的指令</td>
                        </tr>
                        <tr>
                            <td>visible-change</td>
                            <td>下拉框出现/隐藏时触发</td>
                            <td>出现则为 true，隐藏则为 false</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
    
        <el-collapse>
            <el-collapse-item title="Dropdown Menu Item 属性" name="1">
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
                            <td>command</td>
                            <td>指令</td>
                            <td>string/number/object</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                        <tr>
                            <td>disabled</td>
                            <td>禁用</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>divided</td>
                            <td>显示分割线</td>
                            <td>boolean</td>
                            <td>—</td>
                            <td>false</td>
                        </tr>
                        <tr>
                            <td>icon</td>
                            <td>图标类名</td>
                            <td>string</td>
                            <td>—</td>
                            <td>—</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
    </div>
</template>