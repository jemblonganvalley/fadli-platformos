## Firstime Test using Platform OS

Hello, My name's Fadli
This my firt project using platform os,

You can see online result in [here](https://dedicated-fadliselaz.staging.oregon.platform-os.com/)

## About Platform OS
The Platform OS is a Infrastructure as a service platform, where the development of the frontend, backend and ops is simultaneously integrated into one platform.

Actually this process makes all development processes faster, but the problem I found was the lack of resources and documentation for this Platform OS.

For the frontend platform os using a template engine called *liquid*, which is similar to handlebars but in my opinion it has more complete features.

For communication from FE to BE, graphql is used as the bridge, the process is quite easy, we just need to define the schema with the *yml* file format, and sync it with pos-cli, a package that was created to handle the Platform OS from the command line side.

To use this Platform OS, we just need to register on the website [https://www.platformos.com/try-now#content](https://www.platformos.com/try-now#content)

and we are immediately made an instace server that we can choose.

## Installation
You need nodejs package called **pos-cli**, you can find [here](https://www.npmjs.com/package/@platformos/pos-cli).

Or you can type : 
```
sudo npm install -g @platformos/pos-cli
```

and then you can type in coman line :
```bash
pos-cli init
```

Pos-cli will generated basic folder structure.

## Registration Env
For development, you must register your environment
```
pos-cli env add [your repo name] --email [your email] --url [your pOS instance] 
```


> you can choose your repo / env name for example you can choose **demo**


If you havent register to Platform os you can register [here](https://partners.platformos.com/) and create an instance.

## Development
Make a little change in /app/views/index.liquid file, and you can test development stagging url with : 
```
pos-cli sync [repo name] --livereload
```

In Cli we can see our development url, just copy and paste in your browser.
