# A weather lookup service

[Deploy this function on flows.network](#deploy-the-weather-lookup-app), and you will get a web service that using OpenWeatherMap to look weather.

![image](https://user-images.githubusercontent.com/45785633/227089663-7af14499-1860-45a7-ae46-b80b48fc7dfd.png)


This is a simple example to show how [Lambda](https://flows.network/integration/Lambda) works on flows.network.

## Deploy the weather lookup App

To install this weather lookup App, we will use [flows.network](https://flows.network/), a serverless platform that makes deploying your own app quick and easy in just three steps.

## Prerequisite

You will need an OpenWeatherMap API key. If you do not already have one, sign up [here](https://openweathermap.org/appid).

### Fork this repo and write your own code

Fork [this repo](https://github.com/flows-network/weather-lookup). 

### Deploy the code on flow.network

1. Sign up for an account for deploying flows on [flows.network](https://flows.network/). It's free.
2. Click on the "Create a Flow" button to start deploying the web service.
3. Authenticate the [flows.network](https://flows.network/) to access the `wether-lookup` repo you just forked. 

<img width="948" alt="image" src="https://user-images.githubusercontent.com/45785633/226957614-cf386f63-5283-438e-af72-12de1781aa2b.png">


4. Click on the Advanced text and you will see more settings including branch and environment variables. In this example, we have one variable `API_KEY` to fill in, which is the OpenWeatherMap API key.

<img width="899" alt="image" src="https://user-images.githubusercontent.com/45785633/226958901-8824bd5a-e2c9-42cc-9ccd-fbec952535f0.png">

5. Click the Deploy button to deploy your function.

### Configure SaaS integrations

After that, the flows.network will direct you to configure the SaaS integration required by your flow. Here we can see: there is no SaaS needs to be connected since it's a lambda service. Just click the Check button to see your flow details.

<img width="964" alt="image" src="https://user-images.githubusercontent.com/45785633/226959151-0e8a159a-02b3-4130-b7b5-8831b65c8d75.png">


## Try this demo

After the flow function's status becomes `ready`, you will see a link under the Lambda Endpoint. Copy and paste this url to your brower and add `?city=cityname` to look up the city weather you want to know.


![image](https://user-images.githubusercontent.com/45785633/227093331-f19f57a2-e3d9-4b31-97e0-00cfe19b9bda.png)


> [flows.network](https://flows.network/) is still in its early stages. We would love to hear your feedback!


## Others


To build locally, make sure you have intsalled Rust and added `wasm32-wasi` target.

```
cargo build target wasm32-wasi --release
```
