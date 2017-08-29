# microformat-hotels
Examples of Microformats setups for hotels

The aim is to allow search engines (obviously Google in particular) to find MicroFormat values (also know as Knowledge Graph) in order to publish them in the SERP (Search Engine Result Page). In the case of hotels, Google displays stars corresponding the overall rating from customer reviews and the number of votes. Next to this you can also have a basic price information.
This line catch users eyes and increase the CTR (Clic Through Rate).



This example is used in a Google Tag Manager 'Balise'. 



*** Stars that appear in the SERP ***

"aggregaterating": { "@type":"aggregaterating",
               "ratingValue" : "{{hotel.reviewsNote}}",
               "ratingCount" : "{{hotel.reviewsCount}}"
               
If your hotel website is equipped with a customer reviews aggregator (ie, Customer Alliance), you can dev a little push of the main values (Note & Count) in a Datalayer. Then you can set up Google Tag Manager variables to hosts these values and use them in the main JSON.
 
 
 *** Basic Price information next to the Rating & Votes) ***
 
 "priceRange" : "{{hotel.priceRange}}",

Same idea here. You can set it up manually :   "priceRange" : "From 50$ / night",
or you can bring a little dev to push a dynamic data in a Datalayer --> GTM variable




   
