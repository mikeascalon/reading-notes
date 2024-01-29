# Reading Notes

What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

* Improved developer productivity: As noted above, serverless enables development teams to focus on writing code, not managing infrastructure. It gives developers much more time to innovate and optimize their front-end application functionality and business logic.

* Pay for execution only: The meter starts when the request is made, and ends when execution finishes. Compare this to the infrastructure as a service (IaaS) compute model, where customers pay for the physical servers, virtual machines (VMs) and other resources required to run applications, from the time they provision those resources until the time they explicitly decommission them.

* Develop in any language: Serverless is a polyglot environment, enabling developers to code in any language or framework—Java, Python, JavaScript, node.js—with which they're comfortable.

* Streamlined development/DevOps cycles. Serverless simplifies deployment and, in a larger sense, simplifies DevOps because developers don't spend time defining infrastructure required to integrate, test, deliver and deploy code builds into production.

* Cost-effective performance. For certain workloads—embarrassingly parallel processing, stream processing, certain data processing tasks—serverless computing can be both faster and more cost-effective than other forms of compute.

* Usage visibility. Serverless platforms provide near-total visibility into system and user times and can aggregate usage information systematically.

How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

To get started, create an account with Vercel. You can select the plan that's right for you.

* Sign up
If you've never used Vercel before, sign up for a new Vercel account

* Log in
If you already have a Vercel account, log in to get started

Once you create an account, you can choose to authenticate either with a Git provider or by using an email. When using email authentication, you may need to confirm both your email address and a phone number.

Install the Vercel CLI (Command-Line Interface)

```python
Install the Vercel CLI (Command-Line Interface):
```

What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

API stands for application programming interface. In essence, an API acts as a communication layer, or interface, that allows different systems to talk to each other without having to understand exactly what the others do.


What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?


The Requests library in Python is a popular and user-friendly HTTP library that simplifies sending HTTP requests to interact with web services, including APIs. It provides a convenient and straightforward way to send HTTP requests, handle responses, and work with various HTTP methods (e.g., GET, POST, PUT, DELETE). You can use the Requests library to make HTTP requests to retrieve data from external sources, post data, and perform other HTTP-related tasks.

* Installing Requests:

```python
pip install requests

```
Sending a GET Request:
****
```python
import requests

# Define the URL you want to send a GET request to
url = "https://jsonplaceholder.typicode.com/posts/1"

# Send a GET request
response = requests.get(url)

# Check if the request was successful (HTTP status code 200)
if response.status_code == 200:
    # Parse and print the response content (typically JSON or HTML)
    data = response.json()
    print(data)
else:
    print(f"Error: {response.status_code} - {response.text}")

```
****
## Resources

[What is serverless?](https://www.ibm.com/topics/serverless)

[Projects and deployments](https://vercel.com/docs/getting-started-with-vercel/projects-deployments)

[Python & APIs: A Winning Combo for Reading Public Data](https://realpython.com/python-api/)

[ChatGPT](https://chat.openai.com/)