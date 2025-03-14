<template>
    <DocComponent
        title="Vue Form Library"
        header="Forms"
        description="The PrimeVue Forms library provides comprehensive form state management with built-in validation support."
        :componentDocs="docs"
        :apiDocs="['Form', 'FormField']"
        :ptTabComponent="ptComponent"
        :themingDocs="themingDoc"
    />
</template>

<script>
import AccessibilityDoc from '@/doc/forms/AccessibilityDoc.vue';
import BasicDoc from '@/doc/forms/BasicDoc.vue';
import DownloadDoc from '@/doc/forms/DownloadDoc.vue';
import DynamicDoc from '@/doc/forms/DynamicDoc.vue';
import ImportDoc from '@/doc/forms/ImportDoc.vue';
import ResolversDoc from '@/doc/forms/ResolversDoc.vue';
import StatesDoc from '@/doc/forms/StatesDoc.vue';
import SubmitDoc from '@/doc/forms/SubmitDoc.vue';
import ValidateOnDoc from '@/doc/forms/ValidateOnDoc.vue';
import BuiltInDoc from '@/doc/forms/formfield/BuiltInDoc.vue';
import FormFieldDoc from '@/doc/forms/formfield/FormFieldDoc.vue';
import NonPrimeVueDoc from '@/doc/forms/formfield/NonPrimeVueDoc.vue';
import ResolverDoc from '@/doc/forms/formfield/ResolverDoc.vue';
import TemplateDoc from '@/doc/forms/formfield/TemplateDoc.vue';
import PTComponent from '@/doc/forms/pt/index.vue';
import ThemingDoc from '@/doc/forms/theming/index.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'download',
                    label: 'Download',
                    component: DownloadDoc
                },
                {
                    id: 'import',
                    label: 'Import',
                    component: ImportDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'states',
                    label: 'States',
                    component: StatesDoc
                },
                {
                    id: 'resolvers',
                    label: 'Resolvers',
                    component: ResolversDoc
                },
                {
                    id: 'validateon',
                    label: 'ValidateOn',
                    component: ValidateOnDoc
                },
                {
                    id: 'formfield',
                    label: 'FormField',
                    children: [
                        {
                            id: 'formfield-import',
                            label: 'Import',
                            component: FormFieldDoc
                        },
                        {
                            id: 'formfield-built-in',
                            label: 'Built-in',
                            component: BuiltInDoc
                        },
                        {
                            id: 'formfield-non-primevue',
                            label: 'Non PrimeVue',
                            component: NonPrimeVueDoc
                        },
                        {
                            id: 'formfield-resolver',
                            label: 'Resolver',
                            component: ResolverDoc
                        },
                        {
                            id: 'formfield-template',
                            label: 'Template',
                            component: TemplateDoc
                        }
                    ]
                },
                {
                    id: 'submit',
                    label: 'Submit',
                    component: SubmitDoc
                },
                {
                    id: 'dynamic',
                    label: 'Dynamic',
                    component: DynamicDoc
                },
                {
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            ptComponent: PTComponent,
            themingDoc: ThemingDoc
        };
    }
};
</script>
