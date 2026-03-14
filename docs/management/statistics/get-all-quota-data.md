# Get All Quota Data

Documentation renewed! For old docs, visit https://doc.newapi.pro/

Management API — Statistics

## Get All Quota Data

{% hint style="info" %}
Requires Admin Permissions (Admin)
{% endhint %}

Endpoint

GET https://docs.newapi.pro/api/data/

Response

#### 200

Empty

Code samples

{% tabs %}
{% tab title="cURL" %}
```bash
curl -X GET "https://docs.newapi.pro/api/data/"
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
// JavaScript sample (no body)
fetch("https://docs.newapi.pro/api/data/", {
  method: "GET"
}).then(res => {
  console.log(res.status);
  return res.text();
}).then(body => console.log(body));
```
{% endtab %}

{% tab title="Go" %}
```go
// Go sample (no body)
package main

import (
	"fmt"
	"io/ioutil"
	"net/http"
)

func main() {
	resp, _ := http.Get("https://docs.newapi.pro/api/data/")
	defer resp.Body.Close()
	body, _ := ioutil.ReadAll(resp.Body)
	fmt.Println(resp.StatusCode, string(body))
}
```
{% endtab %}

{% tab title="Python" %}
```python
# Python sample (no body)
import requests
resp = requests.get("https://docs.newapi.pro/api/data/")
print(resp.status_code)
print(resp.text)
```
{% endtab %}

{% tab title="Java" %}
```java
// Java sample (no body)
import java.net.*;
import java.io.*;

public class Main {
  public static void main(String[] args) throws Exception {
    URL url = new URL("https://docs.newapi.pro/api/data/");
    HttpURLConnection con = (HttpURLConnection) url.openConnection();
    con.setRequestMethod("GET");
    int status = con.getResponseCode();
    System.out.println(status);
    BufferedReader in = new BufferedReader(new InputStreamReader(con.getInputStream()));
    String inputLine;
    StringBuffer content = new StringBuffer();
    while ((inputLine = in.readLine()) != null) {
      content.append(inputLine);
    }
    in.close();
    con.disconnect();
    System.out.println(content.toString());
  }
}
```
{% endtab %}

{% tab title="C#" %}
```csharp
// C# sample (no body)
using System;
using System.Net.Http;
using System.Threading.Tasks;

class Program {
  static async Task Main() {
    HttpClient client = new HttpClient();
    var resp = await client.GetAsync("https://docs.newapi.pro/api/data/");
    Console.WriteLine((int)resp.StatusCode);
    Console.WriteLine(await resp.Content.ReadAsStringAsync());
  }
}
```
{% endtab %}
{% endtabs %}

Last updated on 3/1/2026

Related

* Get Verification Status: https://docs.newapi.pro/en/docs/api/management/security-verification/verify-status-get
* Get Personal Quota Data: https://docs.newapi.pro/en/docs/api/management/statistics/data-self-get
