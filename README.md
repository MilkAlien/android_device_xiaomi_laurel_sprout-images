# laurel_sprout prebuilt images

## Current images
| Image                                                                                                                                                                                                                                   | Version    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------|
| vendor.img                                                                                                                                                                                                                              | V11.0.16.0 (GLOBAL) |
| abl.img<br>bluetooth.img<br>cmnlib.img<br>cmnlib64.img<br>devcfg.img<br>dsp.img<br>hyp.img<br>imagefv.img<br>keymaster.img<br>modem.img<br>qupfw.img<br>rpm.img<br>storsec.img<br>tz.img<br>uefisecapp.img<br>xbl.img<br>xbl_config.img | V11.0.16.0  |

## How to update vendor image
1. Extract vendor.img from payload.bin
2. Convert img to simg:
```
img2simg vendor.img vendor.simg
ls -la vendor.simg # check size
rm vendor.img && mv vendor.simg vendor.img
```
3. Update vendor-image.mk and README.md with version, fingerprint and desc
