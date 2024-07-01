## 学习资源

* [bilibili](https://www.bilibili.com/video/BV1s3411G7yM/?buvid=Y843DB827A618F0C426DAF2ACA32D03964F1&from_spmid=search.search-result.0.0&is_story_h5=false&mid=ZZGMQA4t%2BMw3rgrLk5QMZg%3D%3D&p=1&plat_id=114&share_from=ugc&share_medium=iphone_i&share_plat=ios&share_session_id=C8DD3784-8E03-48CC-90C3-41AAD4F9E0BF&share_source=WEIXIN&share_tag=s_i&spmid=united.player-video-detail.0.0&timestamp=1719403092&unique_k=ZmSQ475&up_id=95093036)

* https://web.archive.org/web/20210104105406/https://cs61a.org/

* https://www.composingprograms.com/

## TODO

- [ ] Github workflow

## Important concepts

### Closure 

* https://pythontutor.com/cp/composingprograms.html#mode=display


```py

def add(a, b):
    tmp = 123
    def closure():
        nonlocal 
        tmp += 1
        return a+b
    return closure
    
test = add(1,2)
test()
test()
```
* [TS playground](https://www.typescriptlang.org/play/?#code/PTAEHUFMBsGMHsC2lQBd5oBYoCoE8AHSAZVgCcBLA1UABWgEM8BzM+AVwDsATAGiwoBnUENANQAd0gAjQRVSQAUCEmYKsTKGYUAbpGF4OY0BoadYKdJMoL+gzAzIoz3UNEiPOofEVKVqAHSKymAAmkYI7NCuqGqcANag8ABmIjQUXrFOKBJMggBcISGgoAC0oACCbvCwDKgU8JkY7p7ehCTkVDQS2E6gnPCxGcwmZqDSTgzxxWWVoASMFmgYkAAeRJTInN3ymj4d-jSCeNsMq-wuoPaOltigAKoASgAywhK7SbGQZIIz5VWCFzSeCrZagNYbChbHaxUDcCjJZLfSDbExIAgUdxkUBIursJzCFJtXydajBBCcQQ0MwAUVWDEQC0gADVHBQGNJ3KAALygABEAAkYNAMOB4GRonzFBTBPB3AERcwABS0+mM9ysygc9wASmCKhwzQ8ZC8iHFzmB7BoXzcZmY7AYzEg-Fg0HUiQ58D0Ii8fLpDKZgj5SWxfPADlQAHJhAA5SASPlBFQAeS+ZHegmdWkgR1QjgUrmkeFATjNOmGWH0KAQiGhwkuNok4uiIgMHGxCyYrA4PCCJSAA)

```ts
function createMultiplier<T extends any>(multiplier: T) {
    return (input: T) => input * multiplier;
}

const double = createMultiplier<number>(2);
console.log(double(104)); // Outputs: 10

```
