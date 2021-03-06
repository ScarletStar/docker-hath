[hub]: https://hub.docker.com/r/frosty5689/hath/

# frosty5689/hath
[![](https://images.microbadger.com/badges/version/frosty5689/hath.svg)](https://microbadger.com/images/frosty5689/hath "Get your own version badge on microbadger.com")[![](https://images.microbadger.com/badges/image/frosty5689/hath.svg)](https://microbadger.com/images/frosty5689/hath "Get your own image badge on microbadger.com")[![Docker Pulls](https://img.shields.io/docker/pulls/frosty5689/hath.svg)][hub][![Docker Stars](https://img.shields.io/docker/stars/frosty5689/hath.svg)][hub]

## Usage

```
docker run \
  --name hath \
  --net=host \
  -v /path/to/your/hath/cache:/hath/cache \
  -v /path/to/your/hath/data:/hath/data \
  -v /path/to/your/hath/download>:/hath/download \
  -v /path/to/your/hath/log:/hath/log \
  -v /path/to/your/hath/tmp:/hath/tmp \
  -e HATH_CLIENT_ID=YOUR_HATH_CLIENT_ID \
  -e HATH_CLIENT_KEY=YOUR_HATH_CLIENT_KEY \
  -e TZ=YOUR_TIMEZONE \
  frosty5689/hath
```

## Parameters

* `--net=host` - Uses host network with container, use this if H@H have trouble accepting connections. This will let H@H use the host's internal IP for routing instead of the internal IP used by Docker bridge.
* `-v /hath/cache` - H@H cache
* `-v /hath/data` - H@H data
* `-v /hath/download` - H@H download
* `-v /hath/log` - H@H log
* `-v /hath/tmp` - H@H tmp
* `-e HATH_CLIENT_ID` - H@H Client ID
* `-e HATH_CLIENT_KEY` - H@H Client Key
* `-e TZ` - Timezone H@H will run in

