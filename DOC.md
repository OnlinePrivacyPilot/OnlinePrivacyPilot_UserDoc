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

![example_search_form_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/59505383/71872f59-105b-43d0-9048-9141c8c2b15e)

Using these parameters, when you click the "Launch Search" button, it will test the validity of your 
key, taking into account the parameters you specify.
If you are told that your key is not valid, that means either that you have made an error while 
The result we get in our example is as follows:

![example_result_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/59505383/bbbb5cdd-aa69-4c87-83cb-faaf382e300e)

You can see that the number of results is limited to twenty, but it is still a huge set. If we want 
for instance to filter it, we can add filters, either initially or by clicking on a node. If we 
relaunch a search with "Instagram" and "LinkedIn"  we will have:

![example_result_with_filters_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/59505383/01502cc5-d2fd-4679-a08b-c17f767ecdd9)

![example_delete_data_macron](https://github.com/OnlinePrivacyPilot/OnlinePrivacyPilot_UserDoc/assets/59505383/3a37ec8c-9579-4378-b157-a8e18d075be5)

If we click on the node linked to his Instagram account and since we are able to find the procedure 
of deletion for Instagram with JustDeleteMe, a button will appear that allows to remove the 
associated data. It will be redirected to the web page of registration for Instagram and afterward 
the deletion page. As mentioned before, it is also possible to indicate if the targeted footprint is 
relevant, i.e., can be somehow linked to our person. It will appear as a filter in the filters list, 
accessible and usable for potential further searches.


###### Google Custom API creation {#google-api-key-creation}

This section will show you how to create an API key that you can use to make requests to the tool.
The first step is to click [on this link ](https://console.cloud.google.com/), which will take you 
to the Google Console platform. If you are already connected to your account you might see this:

If you are not, it will suggest that you either create one or log in.
The very first step is to create a project. Whatever its name, the project allows you to use 
various APIs and manage your keys and permissions, among other things.

For this example, we will create a project called OnlinePrivacyPilotTest, as shown here:

Once this is done, click on the "Credentials" on the left. It will allow you to create a key by 
clicking on the "API key" field. 

Now that you have your created key, you need to enable an API called "Custom Search API". This 
screenshot shows the activation process:

Congratulations, you are almost done with the creation of your key, the only step that remains is 
to click on "Credentials" on the left and then copy the value of your key to be paste directly into 
the tool.

It is important to mention that behind this project you've created, there's a query limit that can 
be used with the Custom Search API service. You'll be able to generate just 100 queries in 24 hours.
You can monitor your quota in the Google Console, here is an example of an exceed number of query:

