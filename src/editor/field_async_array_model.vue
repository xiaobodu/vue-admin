<template>
    <field_array_model
        v-model="model"
        :candidate="candidate"
        :labelfield="labelfield"
        :valuefield="valuefield"
        :placeholder="placeholder"
    ></field_array_model>
</template>

<script>
import _props_label_value_mixin from "./_props_label_value_mixin.js"
import _async_candidate_mixin from "./_async_candidate_mixin.js"
import _computed_model_mixin from "./_computed_model_mixin.js"
import _props_placeholder_mixin from "./_props_placeholder_mixin.js"
import _props_value_array_mixin from "./_props_value_array_mixin.js"
import field_array_model from "./field_array_model"

export default {
    name:'field_async_array_model',
    mixins:[
        _props_label_value_mixin,
        _async_candidate_mixin,
        _computed_model_mixin,
        _props_placeholder_mixin,
        _props_value_array_mixin,
    ],
    components:{
        field_array_model
    },
    props:{

    }
}
</script>