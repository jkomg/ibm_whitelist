# ibm_whitelist
The Bluemix whitelist shenanigans

1.    Open a Private / Incognito tab or window on your browser

2.    Whitelisting link - [https://cloud.ibm.com/registration/whitelist](https://cloud.ibm.com/registration/whitelist)

3.    Open this link - [https://cloud.ibm.com/healthcheck/v1/status](https://cloud.ibm.com/healthcheck/v1/status)

4.    Take the value of clusterName key from the JSON. For example, "cloud-prod-tok02".

5.    The value after "cloud-prod-" is the Region. In this case, it is tok02

6.    Go to the region-specific whitelisting page by forming a url with the region, like this - [https://tok02.console.cloud.ibm.com/registration/whitelist](https://tok02.console.cloud.ibm.com/registration/whitelist)

7.    Get the short VCPI URL from Federated Advocacy Tool for the event and open it in a browser

8.    For e.g., let's take [https://ibm.biz/BdzEA6](https://ibm.biz/BdzEA6)

9. Opening this link in browser would give this expanded link –
[https://cloud.ibm.com/registration?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank%5Csudharshan-govindan%5Ccgiworkshop-bangalore-05132019-bangalore-5132019-5162019%5CMay2019%5Cworkshop%5Cglobal-devadvgrp-bangalore%5Cbangalore%5Cindia%5C%5Ckubernetes-vs-docker-its-not-an-either-or-question&cm_mmca1=000019RS&cm_mmca2=10004805&cm_mmca3=M99938765&cvosrc=email.Events.M99938765&cvo_campaign=000019RS](https://cloud.ibm.com/registration?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank%5Csudharshan-govindan%5Ccgiworkshop-bangalore-05132019-bangalore-5132019-5162019%5CMay2019%5Cworkshop%5Cglobal-devadvgrp-bangalore%5Cbangalore%5Cindia%5C%5Ckubernetes-vs-docker-its-not-an-either-or-question&cm_mmca1=000019RS&cm_mmca2=10004805&cm_mmca3=M99938765&cvosrc=email.Events.M99938765&cvo_campaign=000019RS)

10. Split the link till "&cm_mmca1". In this case, it will be –
[https://cloud.ibm.com/registration?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank\sudharshan-govindan\cgiworkshop-bangalore-05132019-bangalore-5132019-5162019\May2019\workshop\global-devadvgrp-bangalore\bangalore\india\\kubernetes-vs-docker-its-not-an-either-or-question](https://cloud.ibm.com/registration?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank\sudharshan-govindan\cgiworkshop-bangalore-05132019-bangalore-5132019-5162019\May2019\workshop\global-devadvgrp-bangalore\bangalore\india\\kubernetes-vs-docker-its-not-an-either-or-question)

11. add a slash after "registration" to the above link (this is important!).  so, it will become -
[https://cloud.ibm.com/registration/?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank\sudharshan-govindan\cgiworkshop-bangalore-05132019-bangalore-5132019-5162019\May2019\workshop\global-devadvgrp-bangalore\bangalore\india\\kubernetes-vs-docker-its-not-an-either-or-question](https://cloud.ibm.com/registration/?cm_mmc=Email_Events-_-Developer_Innovation-_-WW_WW-_-mapatank\sudharshan-govindan\cgiworkshop-bangalore-05132019-bangalore-5132019-5162019\May2019\workshop\global-devadvgrp-bangalore\bangalore\india\\kubernetes-vs-docker-its-not-an-either-or-question)

12. In the browser window to which you navigated in step 6, copy the URL from step 11 into the "Custom Registration URL" field, and then click the "Whitelist List" button.  This action will create a whitelisting entry, for the tok02 region, that will whitelist (not block) any user that navigates to cloud.ibm.com/registration with the specified cm_mmc parameter.
