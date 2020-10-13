# Setting up Stripe Subscriptions with Flask

## Want to learn how to build this?

Check out the [post]().

## Want to use this project?

1. Fork/Clone

1. Create and activate a virtual environment:

    ```sh
    $ python3 -m venv venv && source venv/bin/activate
    ```

1. Install the requirements:

    ```sh
    (venv)$ pip install -r requirements.txt
    ```

1. Add your Stripe test secret and publishable keys as environment variables like so:

    ```sh
    (venv)$ export STRIPE_PUBLISHABLE_KEY=<YOUR_STRIPE_PUBLISHABLE_KEY>
    (venv)$ export STRIPE_SECRET_KEY=<YOUR_STRIPE_SECRET_KEY>
    ```

1. In case you're planning to confirm payments using webhooks you also need to add the webhook endpoint environment variable as well:

```sh
(env)$ export STRIPE_ENDPOINT_SECRET=<YOUR_ENDPOINT_SECRET_KEY>
```

1. Run the server:

    ```sh
    (venv)$ FLASK_ENV=development python app.py
    ```

    Navigate to [http://localhost:5000](http://localhost:5000).