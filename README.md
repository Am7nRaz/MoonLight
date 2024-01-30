# My Things 1

First Update your server :

```bash
apt update && apt upgrade -y
```

install ``hiddify`` or ``MHSanaei`` or ``alireza0`` or ``Kafka``:

``hiddify``:

```bash
curl https://install.hiddify.com/release |bash
```
OR
```bash
sudo apt update&&sudo apt install -y curl&& curl -sSL https://raw.githubusercontent.com/hiddify/hiddify-manager/main/common/download.sh | sudo bash -s release
```
``MHSanaei``:

```bash
bash <(curl -Ls https://raw.githubusercontent.com/mhsanaei/3x-ui/master/install.sh)
```
``alireza0``:

```bash
bash <(curl -Ls https://raw.githubusercontent.com/alireza0/x-ui/master/install.sh)
```
``Kafka`` EN VERSION:

```bash
bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/x-ui/master/install_en.sh)
```
Worker code :

```bash
addEventListener(
   "fetch", event => {
       
       const ip = event.request.headers.get('cf-connecting-ip') || event.request.headers.get('x-forwarded-for') || (event.request.socket && event.request.socket.remoteAddress);
       let url = new URL(event.request.url);
       const worker_domain=url.hostname;
       url.hostname = "sub.domain.com";                        
       url.protocol = event.request.headers.get('x-forwarded-proto') || "https";
       let request = new Request(url, event.request);
       if (ip)
        request.headers.set('cf-connecting-ip', ip);
        request.headers.set('Host', worker_domain);
       event.respondWith(
           fetch(request)
       )
   }
)

```

Server Optimizer : 

```bash
sudo apt update -q && sudo apt install -y sudo wget
```
```bash
sudo -i
```
```bash
wget "https://raw.githubusercontent.com/hawshemi/Linux-Optimizer/main/linux-optimizer.sh" -O linux-optimizer.sh && chmod +x linux-optimizer.sh && bash linux-optimizer.sh 
```
Press 1

Online tools i need : 

<a href="https://drunkleen.github.io/xray-fragmenter/" target="_blank"> Fragmenter Site </a>

Download latest software : 

<a href="https://github.com/2dust/v2rayNG/releases" target="_blank"> V2RAYNG Android Releases </a>

<a href="https://github.com/2dust/v2rayN/releases" target="_blank"> V2RAYNG PC Releases </a>

<a href="https://..../releases" target="_blank"> My Own App ( SOON ) </a>
