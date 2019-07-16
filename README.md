# v2ray-custom-geo

## 自定义 geosite.dat & geoip.dat 文件
## 准备
    git clone https://github.com/aljangtze/v2ray-custom-geo.git
    tar -C /usr/local/ -xzf go1.12.7.linux-amd64.tar.gz    
    export PATH=$PATH;/usr/local/go/bin
    export GOPATH=/usr/local/go
    export PATH=$PATH:/usr/local/go/bin
    go get github.com/gogo/protobuf
    go get github.com/v2ray/v2ray-core
    go get go.starlark.net/syntax
### 使用

  - 修改/添加 sites 文件夹下的域名文件，运行 ./v2sitedat 生成 geosite.dat
  - 修改/添加 ips 文件夹下的地址文件，运行 ./v2ipdat 生成 geoip.dat

#### 推荐
  - 国内域名
  https://raw.githubusercontent.com/felixonmars/dnsmasq-china-list/master/accelerated-domains.china.conf
  
  - 国内ip
  https://github.com/17mon/china_ip_list/blob/master/china_ip_list.txt

**改自 https://github.com/onplus/v2ray-SiteDAT
