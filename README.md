# Offline WebSocket System for Laravel and React Projects

Before using Laravel Echo, we were utilizing Laravel Pusher. However, some of our branches did not have internet access due to security policies, so we needed to implement our own offline WebSocket system for our Laravel and React project.

![laravel-offline-websocket](https://github.com/esi-t/laravel-offline-webscoket/assets/148218108/528c314d-7018-4339-92ed-ea6f6404805d)

We utilized Redis Pub/Sub features to transfer our data and messages in real time. Whenever a new request was made, clients would be notified based on their store ID, and their data would be updated accordingly.

You can use Laravel Echo instead, but if you need to implement your own WebSocket system, you can follow this architecture. You can use a different framework or programming language instead of Laravel or React if needed. As long as you implement an architecture similar to this, everything should work fine.
