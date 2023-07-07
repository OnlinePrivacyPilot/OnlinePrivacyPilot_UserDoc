# OnlinePrivacyPiloT User Documentation

###### Global Documentation
On this page we will explain you how to use Online Privacy Pilot with a basic scenario. You will get 
a better overview of what you can do with the tool and its functionalities. It serves as examples to 
guide you through your journey with the tool, but sometimes the small (i) icons next to the elements 
could give you the answer of what you are looking for, you just have to put your mouse over it.

Accessing public information is something that should not be underestimated. You should not use this
tool to obtain information of any kind from a third party. The example here uses the name of a 
well-known person and serves merely as an illustration.

Because we do not want to expose the public information of a casual person, we will use the name 
Emmanuel Macron because he is already famous. The first step is to put his name as an input in the 
"Target" field. We do not want to focus on the filters and their effect so far, we will simply 
specify the options we want to use.

You should enter your API key before moving forward, in this case all the requests you will do will 
be somehow associated with your Google account, think about it twice before using the tool.
[This is the procedure](#google-api-key-creation) to create your Google API key.

An API key, also known as an application programming interface key, is a unique identifier used to 
authenticate and authorize access to an API (application programming interface). Here, creating your
own API key will allow you to obtain information and make queries to the Google Custom API in the 
same way that you would with a basic search engine.

The last options are explained, as the others, in the (i) icon. The Active Search checkbox 
correspond to your willingness of using active OSINT techniques. Finally, the Search Depth specify 
how deep you want the software to investigate. The screenshot below illustrates what we have 
exposed, the API key has been blurred, you will have to put your own.

![example_search_form_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/69c97b59-3cc2-4851-a487-3eec21353083)

Using these parameters, when you click the "Launch Search" button, it will test the validity of your 
key, taking into account the parameters you specify.
If you are told that your key is not valid, that means either that you have made an error while 
The result we get in our example is as follows:

![example_result_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/030ff038-7ace-450d-9809-cd86af94d8ce)


You can see that the number of results is limited to twenty, but it is still a huge set. If we want 
for instance to filter it, we can add filters, either initially or by clicking on a node. If we 
relaunch a search with "Instagram" and "LinkedIn"  we will have:

![example_result_with_filters_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/1100ec73-739f-41de-8f87-9b2d5fcda366)

On the other hand if we find that his Instagram account is not relevant we can click on the
corresponding node, this appears then:

![example_delete_data_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/42618e1e-5411-4e6d-86f0-f8004a659b18)

Since we are able to find the procedure of deletion for Instagram with JustDeleteMe, a button will appear
that allows to remove the associated data. It will be redirected to the web page of registration for
Instagram and afterward the deletion page. 

Regarding our relevance choice, it will appear as a
filter in the filters list, accessible and usable for potential further searches.
In our case, with these parameters:

![example_filters_input_search2_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/ca0ff94a-333e-481f-81e0-67f3b57cadd0)

The nodes containing his footprints linked with Instagram do not appear anymore:

![example_macron_disappear_instagram](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/8ecff7af-e335-4da4-848f-39a43c82571f)



###### Google Custom API creation {#google-api-key-creation}

This section will show you how to create an API key that you can use to make requests to the tool.
The first step is to click [on this link ](https://console.cloud.google.com/), which will take you 
to the Google Console platform. If you are already connected to your account you might see this

![google_console_first_view](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/3ca201d8-cc49-4461-b80a-33ddd737340f)

If you are not, it will suggest that you either create one or log in.
The very first step is to create a project. Whatever its name, the project allows you to use 
various APIs and manage your keys and permissions, among other things.

For this example, we will create a project called OnlinePrivacyPilotTest, as shown here:

![google_console_creation_project](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/5b2280ec-f0a0-449b-b75e-42621e3d836c)

Once this is done, click on the "Credentials" on the left. It will allow you to create a key by 
clicking on the "API key" field. 

![google_console_creation_api_key](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/223b2644-ed6c-457b-8524-5c4a4df8bc04)

Now that you have your created key, you need to enable an API called "Custom Search API". These 
screenshots shows the activation process:

![google_console_activation_API_step1](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/37cc47c3-acf5-4551-a002-af21f41dd10a)

![google_console_activation_API_step2](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/900bd7e2-6a96-4263-8e42-530e37bbc187)

Congratulations, you are almost done with the creation of your key, the only step that remains is 
to click on "Credentials" on the left and then copy the value of your key to be paste directly into 
the tool. (It has been blurred on this screenshot).

![google_console_copy_API_key](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/83447138-05f3-4f91-959a-e0269b56d058)


It is important to mention that behind this project you've created, there's a query limit that can 
be used with the Custom Search API service. You'll be able to generate just 100 queries in 24 hours.
You can monitor your quota in the Google Console, here is an example of an exceed number of query:

![google_console_exceed_quotas](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/100564746/38833949-3f7c-486b-811b-6f25bfc4ec15)



