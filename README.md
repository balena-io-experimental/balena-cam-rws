# resin-cam-rws
A Raspberry Pi streaming camera based on [rpi-webrtc-streamer](https://github.com/kclyu/rpi-webrtc-streamer).

## Getting started

- Sign up on [resin.io](https://dashboard.resin.io/signup) and follow our [Getting Started Guide](https://docs.resin.io/raspberrypi3/nodejs/getting-started/)
- Clone this repository to your local workspace
- Set these variables in the [`Fleet Configuration`](https://docs.resin.io/configuration/advanced/) application side tab
  - `RESIN_HOST_CONFIG_gpu_mem` = `196`
  - `RESIN_HOST_CONFIG_start_x` = `1`
- Add the _resin remote_ to your local workspace by running the useful command from the Resin dashboard
- Push code to your device with a simple `git push resin master`
  - See the magic happening, your device is getting updated Over-The-Air!
- Make sure to update your devices after every change you make! You can either:
  - Commit your changes and do another `git push resin master`
  - Learn more about the powerful [**resin-cli**](https://docs.resin.io/raspberrypi3/nodejs/getting-started/#using-resin-sync-to-develop-fast) and how you can iterate and deploy to your devices rapidly!

    Running a simple `resin sync` in your working directory will sync your changes to local devices faster than a `git push`.

## Finally

To watch your stream visit this link: `http://<raspberrypi>:8889/native-peerconnection/`.
Where `<raspberrypi>` is the IP address of your Pi which can be found in your resin.io account's Dashboard.

## License

Copyright 2018 Resinio Ltd.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
