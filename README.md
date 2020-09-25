# ECE444-F2020-Lab2

This repo is a clone of https://github.com/miguelgrinberg/flasky

## Activity 1

The screenshot below shows a succesful import of `flask` in a virtual environment named `venv`.

![Successful install of Flask in virtual environment](/images/activity-1-success.png)

## Activity 2

The screenshot below shows a successful run of the `hello.py` Flask application. The path of `/user/Amar` greets `Amar` with a customized Hello World message.

![Dynamic routing in hello.py](/images/activity-2-success.png)

## Activity 3

Flask context globals are objects that are available to the view function without explicitly being passed in as an argument. These are like global variables to the programmer, but under the hood they are local to a "context", either:

- *application* context
  - `current_app` and `g` variables
- *request* context
  - `request` and `session` variables

The benefit of contexts is that modifying a "context global" object in one thread will not interfere with other threads. This enables the server to work on different requests from different clients at the same time.
