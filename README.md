<h1 align="center"> How to deploy a smart-contract in Taiko (TR/EN) </h1>
<div align="center">

![image](https://user-images.githubusercontent.com/76253089/213913953-832675ec-a344-4de2-a05c-427306f26d7f.png) 
</div>

<h3> 

[If you have any questions, you can click here to contact me.](https://enzifiri.me/)

</h3>

## You can run it on the server where the taiko is installed, it will not cause any problems.

<details>

<summary> 
<h2> English Guide (Click Here) </summary> </h2>

1- Connect to your VPS/VDS server using terminal. <br>
2- Enter the commands below. 


`apt-get upgrade`  <br>
`apt install curl` <br>
`apt install get` <br>
`curl -L https://foundry.paradigm.xyz | bash` <br>
`source /root/.bashrc` <br>
`foundryup` <br>
`mkdir taiko` <br>
`cd taiko` <br>
`git config --global user.email "you@example.com"` <br>
`git config --global user.name "Your Name"` <br>
`forge init enzifiri --force` <br>
`cd enzifiri` <br>
`forge build` <br>
(Combine the commands below.) <br>
`forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key METAMASKPRIVATEKEY src/Counter.sol:Counter` <br>



Replace METAMASKPRIVATEKEY with your private wallet key. <br>

Congratulations, if you see the tx hash in your output, you have successfully created your contract. You can view the output from explorer. <br>

<h2> 

[Taiko Explorer Link](https://l2explorer.a1.taiko.xyz/)

</h2>


</details>


<summary> 

<h2> Türkçe Rehber </summary> </h2>

## Taikonun kurulu olduğu sunucuda çalıştırabilirsiniz, herhangi bir problem yaratmaz.

1- Terminal kullanarak VPS/VDS sunucunuza bağlanın <br>
2- Aşağıdaki komutları sırasıyla yazın. 


`apt-get upgrade`  <br>
`apt install curl` <br>
`apt install get` <br>
`curl -L https://foundry.paradigm.xyz | bash` <br>
`source /root/.bashrc` <br>
`foundryup` <br>
`mkdir taiko` <br>
`cd taiko` <br>
`git config --global user.email "you@example.com"` (Mail Girin)<br> 
`git config --global user.name "Your Name"`(isim girin) <br>
`forge init enzifiri --force` <br>
`cd enzifiri` <br>
`forge build` <br>
(alttaki komutları birleşik yazın) <br>
``` forge create --legacy --rpc-url https://rpc.a2.taiko.xyz --private-key METAMASKPRIVATEKEY src/Counter.sol:Counter ``` <br>
Aldığınız çıktıyı Explorerda aratın başarıylı ise sorun yoktur. (Son komutu 3 4 kere calıstırdım nolur ne olmaz :)))

METAMASKPRIVATEKEY yazan yere Cüzdanınızın private keyini girin ve komutu çalıştırın <br>

Eğer çıktıda TX çıktısı görüyorsanız muhtemelen başarılı şekilde contratı oluşturdunuz. Verdiği txi Explorerda aratıp kontrol edin. <br>

## Hata alırsanız oluşturduğunuz taiko klasörünü silip tekrar komutları girin (source ile başlayan komutla başlayın) <br>

Taiko klasörünü silme komutu `rm -rf taiko`

<h2> 

[Taiko Explorer Link](https://l2explorer.a2.taiko.xyz/)

![image](https://user-images.githubusercontent.com/76253089/227777027-ef64e3f3-3d73-4893-beb3-757e564ce005.png)

</h2>
