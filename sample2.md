# exercise

## 利害關係人表

| 利害關係人 | 目標 |
| -- | -- |
| 人員 | 可以用Line加入業務員的群組 |
|  | 可以使用業務員的會員註冊 |
|  | 可以使用業務員/系統維護員的業務員註冊連結 |
|  | 能夠創建註冊資料與拍照等待核准註冊 |
| 會員 | 可以修改自己部分資料 |
|  | 能夠在進場藉由臉部辨識系統與照片做比對，確認是否為會員 |
|  | 可以確認為會員則可進入場地 |
|  | 可以確認不為會員則不可進入場地 |
|  | 能夠在繳費前一周與未繳費過期隔天收到簡訊通知 |
| 業務員 | 可以修改自己部分資料 |
|  | 可以用Line創群組拉會員加入 |
|  | 能夠用Line發送會員註冊連結 |
|  | 能夠用Line發送業務員註冊連結 |
|  | 能夠批准將成為會員/業務員的會員註冊 |
|  | 能夠在進場藉由臉部辨識系統與照片做比對，確認是否為業務員 |
|  | 可以確認為業務員則可進入場地 |
|  | 可以確認不為業務員則不可進入場地 |
| 系統管理員 | 能夠在系統灌好時預設於資料庫中 |
|  | 可以用Line創群組拉人員加入 |
|  | 可以用Line發送業務員註冊連結 |
|  | 能夠批准將成為會員/業務員的會員註冊 |

## 事件表

| 事件 | 使用案例 |
| -- | -- |
| 1.業務員與系統管理員可以用Line創建群組加入人員進入群組 | 1.連結收發流程 |
| 2.業務員可以用Line發送會員註冊連結 |  |
| 3.業務員與系統管理員可以用Line發送業務員註冊連結 |  |
| 4.人員能夠點擊連結進行註冊 | 2.註冊流程 |
| 5.人員能填寫註冊資料與拍照等待批准 |  |
| 6.所有人可以於系統中進行登入系統 | 3.登入流程 |
| 7.所有人能於系統中修改自己部分資料 | 4.基本資料作業 |
| 8.會員與業務員可以藉由第三方臉部辨識系統與照片比對確認身分 | 5.臉部辨識核對作業 |
| 9.身分為業務員或系統管理員可以進入場地，不為則不可進入 |  |
| 10.身分為會員且為該會員的進場時間，可進入場地，不為則不可進入 |  |
| 11.在要付費的前一周能透過華鐘電信發送簡訊給該會員 | 6.簡訊訊息作業 |
| 12.若未能付費，在付費過期隔天發送提示訊息給會員 |  |
| 13.會員能透過綁訂於騎華銀行的帳戶進行自動扣款 | 7.金流流程 |
| 14.在繳費過期隔天，發送未繳費名單給臉部辨識系統 |  |
| 15.業務員可以透過系統批准將成為會員的人員的註冊 | 8.會員作業 |
| 16.業務員可以透過系統批准將成為業務員的人員的註冊 |  |
| 17.系統管理員可以透過系統批准將成為業務員的人員的註冊 |  |

## 使用案例

| 使用案例名稱 | 連結收發流程 |
| -- | -- |
| 使用案例描述 | 可以發送兩種連結，點擊進系統 |
| 主要參與者 | 人員、業務員、系統管理員 |
| 利害關係人與目標 | 業務員: 可以發送一般註冊與協助註冊兩種連結給人員 |
|  | 系統管理員: 可以發送協助註冊給將成為業務員的人員 |
| 前置條件 | 須先與人員建立Line群組 |
| 後置條件 | 使人員能導向系統進行註冊 |
| 主要成功情節 | 1.人員與業務員或系統管理員先用Line建立群組關係 |
|  | 2.人員點擊被發送的連結 |
|  | 3.人員進入系統 |
| 例外情節 | 無 |
| 其他需求 | 發送的連結可區分一般註冊與協助註冊，業務員與系統人員可依人員將成為身分作發送 |

| 使用案例名稱 | 註冊流程 |
| -- | -- |
| 使用案例描述 | 可讓人員於系統進行註冊 |
| 主要參與者 | 人員 |
| 利害關係人與目標 | 人員: 可以進入系統成功完成申請註冊 |
| 前置條件 | 需先點擊連結進入系統: include 連結收發流程 |
|  | 需引入會員資料: include 會員作業 |
| 後置條件 | 使人員可以於系統中成功完成申請註冊 |
| 主要成功情節 | 1.當人員於系統介面時，可以點擊註冊按鈕 |
|  | 2.該於註冊介面輸入帳號、手機號碼、密碼與再次確認密碼輸入 |
|  | 3.於照片欄位拍照或上傳一張照片 |
|  | 4.可於其他欄位輸入生日、健身取向、習慣運動時間 |
|  | 5.點擊完成註冊 |
| 例外情節 | 無 |
| 其他需求 | 當輸入帳號時動態確認該帳號是否已經於會員資料: include 會員作業 已註冊過 |
|  | 密碼需確認字串中需符合英文大小寫、數字與特殊符號，密碼長度需於8~16字元 |
|  | 如果密碼與再次確認密碼輸入不相同，將再次輸入密碼框顯示紅色，並顯示「兩次密碼不相同，請再次輸入」，且完成註冊按鍵不進行生效 |
|  | 手機號碼需符合全數字，長度需為10字元 |
|  | 當上傳、拍照時動態確認該照片是否有人類特徵 |
|  | 帳號、手機號碼、密碼、再次確認密碼與照片欄皆為必填欄位，皆不可為空 |

| 使用案例名稱 | 登入流程 |
| -- | -- |
| 使用案例描述 | 可讓人員、會員、業務員、系統管理員進行登入 |
| 主要參與者 | 人員、會員、業務員、系統管理員 |
| 利害關係人與目標 | 讓人員、會員、業務員、系統管理員於系統進行登入 |
| 前置條件 | 需引入會員資料: include 會員作業 |
| 後置條件 | 讓人員、會員、業務員、系統管理員可於系統進行登入 |
| 主要成功情節 | 1.點擊login in進入登入畫面 |
|  | 2.輸入帳號、密碼進行登入 |
|  | 3.將輸入字串與會員資料: include 會員作業作比對 |
|  | 4.若登入成功將跳轉到系統主畫面，且login in改為login out |
| 例外情節 | *4a.若登入失敗則顯示「該帳號密碼輸入有誤，請重新輸入」，並保留帳號、清空密碼欄位 |
| 其他需求 | 無 |

| 使用案例名稱 | 基本資料作業 |
| -- | -- |
| 使用案例描述 | 讓會員、業務員、系統管理員對基本資料進行新增、刪除、修改、讀取 |
| 主要參與者 | 會員、業務員、系統管理員 |
| 利害關係人與目標 | 讓會員、業務員、系統管理員於系統對基本資料進行新增、刪除、修改、讀取 |
| 前置條件 | 需引入會員資料: include 會員作業 |
| 後置條件 | 讓會員、業務員、系統管理員可以在系統對基本資料進行新增、刪除、修改、讀取 |
| 主要成功情節 | 1.點擊基本資料進入畫面 |
|  | 2.點擊修改必填欄位 |
|  | 3.可在必填欄位修改帳號、手機號碼、密碼、再次確認密碼 |
|  | 4.點擊修改其他欄位 |
|  | 5.可在其他欄位填入、修改、刪除生日、健身取向、習慣運動時間 |
|  | 6.修改資料均需填入舊密碼作確認 |
|  | 7.點擊完成修改 |
|  | 8.將輸入資料與會員資料: include 會員作業作比對 |
|  | 9.若修改成功將跳轉回系統主畫面 |
|  | 10.將原本的基本資料改為修改完成的資料 |
| 例外情節 | *9a.若修改失敗則顯示「您的部分資料有誤，請填入再作修改」，並保留先前填入欄位、清空舊密碼欄位 |
| 其他需求 | 重新修改帳號時動態確認該帳號是否已經於會員資料: include 會員作業 已註冊過 |
|  | 重新修改密碼時，若密碼與再次確認密碼輸入不相同，將再次輸入密碼框顯示紅色，並顯示「兩次密碼不相同，請再次輸入」，且完成修改按鍵不進行生效 |
|  | 密碼需確認字串中需符合英文大小寫、數字與特殊符號，密碼長度需於8~16字元 |
|  | 重新修改手機號碼時，需符合全數字，長度需為10字元 |
|  | 若舊密碼、帳號、密碼為空，則顯示「為必填欄位，請輸入字串」 |

| 使用案例名稱 | 臉部辨識核對作業 |
| -- | -- |
| 使用案例描述 | 包括以下功能:(1)讓會員、業務員、系統管理員可經過臉部辨識系統自動核對身分(2)核對後判別是否能入場 |
| 主要參與者 | 會員、業務員、系統管理員 |
| 利害關係人與目標 | 會員: 進場時先核對身分，並與會員資料: include 會員作業核對是否為該會員進場時間，若皆是則讓其入場 |
|  | 業務員、系統管理員: 進場時先核對身分，若為是則讓其入場 |
| 前置條件 | 需引入會員資料: include 會員作業 |
| 後置條件 | (1)根據臉部辨識系統與會員資料: include 會員作業作核對身分(2)核對身分判別是否能入場 |
| 主要成功情節 | 1.會員、業務員、系統管理員進入場地將臉靠近相機 |
|  | 2.臉部辨識系統將影像與會員資料: include 會員作業 中的照片作核對身分 |
|  | 3.於include 會員作業中核對身分 |
|  | 4.若為業務員、系統人員則可進入 |
|  | 5.為會員則與會員資料: include 會員作業中的入場時間作核對 |
|  | 6.若為該會員入場時間則可進入 |
| 例外情節 | *4a.若不為業務員、系統人員則判別是否為會員 |
|  | *5a.若不為會員則不可進入 |
|  | *6a.若為會員但不為該會員進場時間則不可進入 |
| 其他需求 | 偵測到該會員、業務員、系統管理員，於電腦中顯示人員身分、編碼與進場時間的綠色字串 |
|  | 偵測到不為會員，則於電腦中顯示該人員為「未註冊人員」的紅色字串 |
|  | 偵測到為會員但不為該會員進場時間，則於電腦中顯示該人員身分、編碼與「不為進場時間」的黃色字串 |

| 使用案例名稱 | 簡訊訊息作業 |
| -- | -- |
| 使用案例描述 | 包括以下功能:(1)臉部辨識系統: include 臉部辨識核對作業在該付費的前一周將其會員名字: include 會員作業中的手機號碼傳給華鐘電信，並由華鐘電信傳送簡訊訊息給該會員(2)臉部辨識系統: include 臉部辨識核對作業接收未繳費會員並轉發給華鐘電信在進行一次傳送簡訊訊息 |
| 主要參與者 | 會員 |
| 利害關係人與目標 | 會員可以在繳費的前一周與過期後一天接收到簡訊訊息提醒 |
| 前置條件 | 需引入會員資料: include 會員作業 |
|  | 需引入臉部辨識系統: include 臉部辨識核對作業 |
| 後置條件 | 使客戶能接收到簡訊訊息 |
| 主要成功情節 | 1.在繳費前一周臉部辨識系統: include 臉部辨識核對作業與會員資料: include 會員作業發送會員名字與手機號碼給華鐘電信 |
|  | 2.華鐘電信根據手機號碼與會員名字發送簡訊訊息給該繳費會員 |
|  | 3.在繳費過期隔天，騎華銀行會發送給臉部辨識系統: include 臉部辨識核對作業未繳費名單 |
|  | 4.若名單不為空，臉部辨識系統: include 臉部辨識核對作業再將未繳費名單發送給華鐘電信 |
|  | 5.華鐘電信根據會員名字與本季名單核對並發送簡訊訊息給會員 |
| 例外情節 | *4a.若名單為空，則臉部辨識系統: include 臉部辨識核對作業不作發送的動作 |
| 其他需求 | 在臉部辨識系統: include 臉部辨識核對作業第一次發送名單給華鐘電信時，自動附註為提醒訊息，在過期隔天，自動附註為未繳費訊息 |

| 使用案例名稱 | 金流流程 |
| -- | -- |
| 使用案例描述 | 包括以下功能:(1)在繳費時間，自動對綁訂於騎華銀行帳戶的會員自動扣款或未綁訂的會員可進行轉帳(2)會員名單有未繳費的會員，在過期隔天騎華銀行將名單發送到臉部辨識系統: include 臉部辨識核對作業 |
| 主要參與者 | 會員 |
| 利害關係人與目標 | 會員可針對「未繳費的款項」進行自動扣款或轉帳扣款 |
| 前置條件 | 臉部辨識系統: include 臉部辨識核對作業傳送會員的繳費期限與編號給騎華銀行 |
| 後置條件 | 根據騎華銀行判定該會員是否繳費完成，來決定臉部辨識系統: include 臉部辨識核對作業的繳費狀態 |
| 主要成功情節 | 1.將臉部辨識系統: include 臉部辨識核對作業應繳費會員資料傳給騎華 |
|  | 2.會員可與騎華銀行綁訂自動扣款或轉帳扣款 |
|  | 3.等待騎華的回應 |
|  | 4.若繳費成功的會員，則改變臉部辨識核對作業的繳費狀態 |
| 例外情節 | *4a.若有會員未繳費，則回應未繳費名單，不改變繳費狀態 |
|  | *4b.未改變繳費狀態臉部辨識核對作業再轉發給華鐘電信 |
| 其他需求 | 無 |

| 使用案例名稱 | 會員作業 |
| -- | -- |
| 使用案例描述 | 包括以下功能:(1)已註冊的業務員以及系統管理員可以批准註冊名單(2)提供會員的基本資料(3)刪除提前解約的會員 |
| 主要參與者 | 業務員、系統管理員 |
| 利害關係人與目標 | 業務員、系統管理員:可以批准人員的註冊 |
|  | 系統:提供會員的基本資料 |
|  | 系統管理員:能對提前解約的會員進行刪除 |
| 前置條件 | 需完成登入: include 登入流程 |
| 後置條件 | 包含(1)批准的人員的註冊(2)提供會員的基本資料(3)刪除提前解約的某會員資料 |
| 主要成功情節 | 1.業務員、系統管理員登入後: include 登入流程可批准人員對註冊流程的註冊 |
|  | 2.若批准成功後，人員成為會員 |
|  | 3.系統管理員可以對提前解約的會員進行刪除 |
|  | 4.刪除成功後，會員從資料庫移除 |
| 例外情節 | *2a.若失敗則將其註冊移除 |
| 其他需求 | 可以提供系統查詢會員的資料 |
