<template>
    <v-container>
        <v-row>
            <v-col cols="12" md="2">
            </v-col>
            <v-col cols="12" md="8">

                <v-banner>
                    <v-container fill-height fluid>
                        <v-row align="center"
                            justify="center">

                            <v-col cols="12" md="2">

                                <v-container fill-height fluid>
                                    <v-row align="center"
                                        justify="center">
                                            <img
                                                src="https://dataportal-data.s3-ap-southeast-2.amazonaws.com/static/images/test_logo.PNG"
                                                alt="sm4_logo"
                                                width="250"
                                            >
                                    </v-row>
                                </v-container>
            
                            </v-col>   
                            
                            <v-col cols="12" md="8">
                                <h2>Dataportal release notes v1.1</h2>
                                <br>
                                <h3 style="color: #6A76AB; font-weight: 300;">What's new in version 1.1?</h3> 
                            </v-col>  

                            <v-col cols="12" md="2">
                                <v-container >
                                    <a href="http://api.stemformatics.org" target="_blank" style="text-decoration: none;">
                                        <v-row >
                                            <v-btn tile block depressed color="#6A76AB" class="white--text">Try</v-btn>
                                        </v-row>
                                    </a>
                                </v-container>
                            </v-col> 
                                       
                        </v-row>
                    </v-container>
                </v-banner>

                <div>
                    <v-container >
                        <v-row >
                            <v-col cols="12" md="10">
                                <v-list>
                                    <v-list-item>
                                        <v-list-item-content>

                                            <v-list-item-title>
                                                <h4 style="font-weight: 400;">What's new</h4> 
                                            </v-list-item-title>
                                           
                                            <v-list-item-content>
                                                <ul>
                                                    <li>
                                                        <p style="color: grey; font-weight: 100;">
                                                        New API routes: You can use a 'lookup' route to check the status of a dataset (private or publicly accessible). 
                                                        Private routes are now available for samples, metadata and expression files for all datasets. 
                                                        </p>
                                                    </li>
                                                    <li>
                                                        <p style="color: grey; font-weight: 100;">
                                                        Security: JWT (Json Web Tokens) are now available for use on the API documentation page. You can request a JWT with the link at the top of the
                                                        page. This token can be used to access private data from the API. Only registered dataportal users will have access to this feature. 
                                                        </p>
                                                    </li>
                                                    <li>
                                                        <p style="color: grey; font-weight: 100;">
                                                        Search: The datasets /annotation page search functionality has been upgraded to allow searching for datasets by sample type. You can type 'MSC', 'iPSC' etc. or any
                                                        known sample type as a search term and return datasets containing these terms. 
                                                        </p>
                                                    </li>
                                                    <li>
                                                        <p style="color: grey; font-weight: 100;">
                                                        Annotation: All datasets are now 'locked' by default. Before you begin annotating a dataset you will be asked to assign yourself to it. 
                                                        Each dataset can have only one annotator assigned at a time. I've also added a feature in the sys admin panel to allow administrators 
                                                        to remove an annotator from a dataset, or transfer ownership of that dataset to another annotator. 
                                                        </p>
                                                    </li>
                                                    <li>
                                                        <p style="color: grey; font-weight: 100;">
                                                        Bugs: I've fixed an issue with downloading expression files from the API - hard coded 'key' 
                                                        parameters in model/datasets,py containing the 'raw' value have been removed in favour of key params provided by the users request. 
                                                        </p>
                                                    </li>
                                                </ul>
                                            </v-list-item-content>
                                       
                                        </v-list-item-content>
                                    </v-list-item>
                                </v-list>  
                            </v-col> 
                            
                            <v-col cols="12" md="2">
                            </v-col>  
                                       
                        </v-row>
                    </v-container>
                </div>

            </v-col>

            <v-col cols="12" md="2">
            </v-col>
        </v-row>
    </v-container>

  
</template>

<script>
export default {
    
}
</script>

<style scoped>

</style>