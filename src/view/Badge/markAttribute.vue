<template>
<div>
    <el-collapse accordion>
        <el-collapse-item title="标记属性" name="1">
            <table >
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
                        <td>value</td>
                        <td>显示值</td>
                        <td>string, number</td>
                        <td>—</td>
                        <td>—</td>
                    </tr>
                    <tr>
                        <td>max</td>
                        <td>最大值，超过最大值会显示 '{max}+'，要求 value 是 Number 类型</td>
                        <td>number</td>
                        <td>—</td>
                        <td>—</td>
                    </tr>
                    <!-- <tr>
                        <td>is-dot</td>
                        <td>小圆点</td>
                        <td>boolean</td>
                        <td>—</td>
                        <td>false</td>
                    </tr> -->
                    <tr>
                        <td>hidden</td>
                        <td>隐藏 badge</td>
                        <td>boolean</td>
                        <td>—</td>
                        <td>false</td>
                    </tr>
                    <tr>
                        <td>type</td>
                        <td>类型</td>
                        <td>string</td>
                        <td>primary / success / warning / danger / info</td>
                        <td>—</td>
                    </tr>
                </tbody>
            </table>
        </el-collapse-item>

    </el-collapse>
</div>
</template>

<script>
export default {
    data() {
        return {}
    }
};
</script>
