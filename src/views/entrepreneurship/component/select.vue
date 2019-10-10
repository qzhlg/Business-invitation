<template>
    <div>
        <el-input v-model="input" :placeholder="vname[1]" size="medium" class="ipt"></el-input> -
        <el-input v-model="input" :placeholder="vname[0]" size="medium" class="ipt"></el-input>
    </div>
</template>
<script>
export default {
    props:['vname']
}
</script>
<style lang="scss" scoped>
.ipt{
    width:130px;
}
</style>