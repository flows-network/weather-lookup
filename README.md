# A Weather lookup service

[Deploy this function on flows.network](#deploy-weather-lookup-app), and you will get a web service that using OpenWeatherMap to look weather.



This is a simple example to show how [Lambda]() works on flows.network.

## Deploy Weather lookup App


To install this Slack calulator App, we will use [flows.network](https://flows.network/), a serverless platform that makes deploying your own app quick and easy in just three steps.

## Prerequisite

You will need an OpenWeatherMap API key. If you do not already have one, sign up [here](https://openweathermap.org/appid).

### Fork this repo and write your own code

Fork [this repo](https://github.com/flows-network/weather-lookup). 

### Deploy the code on flow.network

1. Sign up for an account for deploying flows on [flows.network](https://flows.network/). It's free.
2. Click on the "Create a Flow" button to start deploying the ChatGPT GitHub APP
3. Authenticate the [flows.network](https://flows.network/) to access the `wether-lookup` repo you just forked. 

<img width="948" alt="image" src="https://user-images.githubusercontent.com/45785633/226957614-cf386f63-5283-438e-af72-12de1781aa2b.png">


4. Click on the Advanced text and you will see more settings. Fill in the required Environment Variables. In this example, we have one variable: `API_KEY` to fill in, which is the OpenWeatherMap API key.

<img width="899" alt="image" src="https://user-images.githubusercontent.com/45785633/226958901-8824bd5a-e2c9-42cc-9ccd-fbec952535f0.png">

5. Click the Deploy button to deploy your function.

### Configure SaaS integrations

After that, the flows.network will direct you to configure the SaaS integration required by your flow. Here we can see: there is no SaaS needs to be connected since it's a lambda service. Just click the Check button to see your flow details.

<img width="964" alt="image" src="https://user-images.githubusercontent.com/45785633/226959151-0e8a159a-02b3-4130-b7b5-8831b65c8d75.png">





> [flows.network](https://flows.network/) is still in its early stages. We would love to hear your feedback!


## Others


To build locally

```
cargo build target wasm32-wasi --release
```
