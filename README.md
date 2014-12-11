web-client-sample
=================

The `web-client-sample` shows:

1. How to **authenticate** a user with the `3cixty platform`.
2. How to **revoke** a `3cixty access token`.
3. How to **refresh** a `3cixty token`.
4. How to **check permission** for a `3cixty access token`.

Get started
================
1. `git clone https://github.com/3cixty/web-client-sample.git`

2. Get your `appkey` from 3cixty platform. If you don't know how to get the `appkey`, please have a look at [here] (https://github.com/3cixty/appchallenge). Suppose that you set callback URL of your `appkey`to `http://localhost:8080/web-client-sample/webcome.html`

3. Replace **line 16** in the [login.html] (https://github.com/3cixty/web-client-sample/blob/master/login.html) file with your `appkey`.

4. Copy `web-client-sample` to the WebApps root of your server which listens at the 8080 port for example.

Notes
================
1. `login.html` is front page of the sample. The sample checks whether or not a user signs in by using information at URL location.

2. `welcome.html` is callback URL. Whenever OAuth server calls this callback to give back a 3cixty access token to applications, the callback will refresh the front page so that the front page knows who signs in.
