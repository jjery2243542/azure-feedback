# azure-feedback

我是這門課負責幫同學開帳號，管理額度的助教。這篇心得主要會寫管理介面上覺得的一些感想。也很感謝微軟提供這樣的資源，解決很多同學的困擾。

##### 缺少開多個帳號的使用方式
這門課有100多個學生修課，並且有80幾位學生需要使用這個雲端平台。但加subscription的方式卻只能一個一個加，而且每加一個就需要等5min，這件事會讓開帳號有點麻煩。希望能有相關的機制，能夠一次加入多個subscription.

##### 新增email也只能手動執行
加了subscription之後，也只能夠一個一個加入email帳號(加入多個的api似乎有點bug，常常加完之後又跳回去)，這方面我建議可以增加一個csv檔來加帳號的方法，再使用上會節省許多時間。

##### 新的管理介面沒有用email搜尋的功能
原本的介面會直接顯示email帳號，因此可以在網頁上搜尋同學的email，來找出對應的帳號，現在的介面卻只能看到name，會有點不方便。變成管理方要去查一個有所有資訊的對應表，再去找是哪個subscription.

##### email不能使用學校信箱
一開始不知道這件事，後來同學反應沒辦法開帳號，只好再蒐集一次大家的email，再做一次第2點的流程。但這件事比較次要，只是因為我一開始不知道XD

##### 使用GPU的VM，在說明上不清楚
一開始選擇地區的地方，只有選擇美國東部(和少數一些地方)，才能夠使用有GPU的instance，這件事並沒有在azure官方的文件上看到(或者不容易發現)，我是google好久才找到有人有同樣疑問的，建議可以在容易發現的地方上附註這件事。

##### 安裝套件上
因為使用dl套件需要安裝cuda等東西，這次的作法是，我這邊寫一個script讓大家執行，這部份其實我沒什麼意見，不過不知道你們願不願意在選擇上，就增加一個instance，安裝好cuda和tensorflow, pytorch等DL所需的套件讓大家可以比較方便的使用。

##### 使用完必須關機才不會浪費金額
一開始我沒有好好宣導這件事，導致大家開了之後，就放到沒錢，造成金額上的浪費。不過這件事也有點不方便，也有些同學因為沒有這麼做，就一直浪費錢。這件事在下學期會加強宣導，避免金額的浪費。另外也建議可以增加一些休眠的api，來避免這些不便。

##### 剩下的金額沒有即時更新功能
很多同學因為這樣，放到沒錢，就打不開了。造成在deadline前，管理方必須要一直為了這些同學去幫他們增加額度，免得他們的程式或模型卡在VM上面。希望能有相關的機制，來讓使用者知道現在剩下多少額度，或者是加快更新的頻率。

