# 第一次作業

##### Data Sources 

---
從哪個API來的？
  >TwitterAPI

  內容主題為何？
  > 動畫
  
  下哪個查詢字串？
  > #Animation

##### 收集到的Data Format(JSON的欄位架構）
　
```
 * "contributors": 有TWEET的創辦人，裡面有幫助TWEET名單，是一種集合物件
 * "truncated": 去判定TWEET是否要被減掉，最多不超過140字
 * "text": 文字的內容
 * "is_quote_status": 這篇TWEET的引用狀態,
 * "in_reply_to_status_id": 若這篇TWEET適用於回覆上一人的TWEET，則會顯示原PO的ID,
 * "id":這篇TWEET的ID，若容量大於53BIT時，某些語言會不好解譯,
 * "favorite_count": 顯示這篇TWEEY有多少個LIKE,
 *  "entities": 
    * "symbols": 用$符號讓字串更明顯，類似FACEBOOK的#，一種HASHTAG用法,
    * "user_mentions": 有沒有提到其他有帳戶的暱稱,
    * "hashtags": 這篇TWEET裡面使用到的標籤,
    * "urls": 在這篇TWEET裡面的網址
 *  "retweeted": 用瑜表示這篇TWEET是否有被其他TWITTER分享,
 *  "coordinates": 這個TWEET當時的發文座標,
 *  "source": ,
 *  "in_reply_to_screen_name": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet名稱
 *  "in_reply_to_user_id": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet的使用者ID（以整數表示）,
 *  "retweet_count": 這篇Tweet被轉推的次數,
 *  "id_str": 這篇Tweet的ID,
 *  "favorited": 這篇TWEET是否有被認證完畢的使用者案LIKE,
 *  "user": 
    * "follow_request_sent": 可為空值，是否有已驗證的使用者要求追蹤這位受到保護的使用者帳戶,
    * "has_extended_profile": 有無額外的PROFILE,
    * "profile_use_background_image": USER去決定其他USER是否能使用他們上傳的背景圖片,
    * "default_profile_image": 用於使用者是否有上傳個人照，沒有的話預設為蛋型圖片,
    * "id": 這篇TWEET的ID，若容量大於53BIT時，某些語言會不好解譯,
    * "profile_background_image_url_https":USER若有用背景圖片，這邊會顯示網址,
    * "verified": 使用者驗證是否完成,
    * "profile_text_color": USER使用的字體顏色(以16進位表示),
    * "profile_image_url_https":使用者圖片的網址,
    * "profile_sidebar_fill_color": 使用者使用的側邊欄位的背景顏色（十六進位）,
    * "entities": Entity會顯示有關這篇TWEET的額外資訊
       * "description": 
          * "urls": 這篇TWEET裡面有的網址
    * "followers_count": 顯示這個帳號的追蹤人數,
    * "profile_sidebar_border_color": USER使用的邊框顏色,
    * "id_str": 以字串表示的使用者
    * "profile_background_color": USER用的背景顏色(16進位表示)
    * "listed_count": USER有的LIST數量,
    * "is_translation_enabled": 使用者決定是否允許別人翻譯,
    * "utc_offset": 與標準時間GMT的時差，用秒顯示,
    * "statuses_count": USER發出的TWEET數量,
    * "description": USER的自我介紹,
    * "friends_count": 這個帳號使用者追蹤其他帳號使用者的數量,
    * "location": USER能夠自己定義位置的名稱,
    * "profile_link_color": USER用的超連結顏色,
    * "profile_image_url":USER使用的圖片網址,
    * "following": USER是否有被其他USER追蹤,
    * "geo_enabled": USER能夠選取是否顯示地理位置在圖片上,
    * "profile_background_image_url":USER的背景圖片網址,
    * "screen_name": USER能自行定義名稱，並且能任意更改,
    * "lang": 以BCP47編碼顯示選擇顯示介面的語言,
    * "profile_background_tile": 是否顯示user背景圖片的網址,
    * "favourites_count": user點LIKE的TWEET數量,
    * "name":USER顯示的暱稱，能夠任意更改,
    * "notifications": 是否允許收到SMS的更新通知，當USER發布新TWEET時,
    * "url": USER提供的網址,
    * "created_at": 此USER帳號當初創辦的時間,
    * "contributors_enabled": USER有沒有連結貢獻者模式(contributor mode),
    * "time_zone": user自行定義的時區位置,
    * "protected": user能選擇帳號的隱私程度,
    * "default_profile": user是否有用預設照片,
    * "is_translator": user是否有加入幫忙TWITTER翻譯的工作,
 *  "geo": 不贊同使用，現在都使用coordinates欄位紀錄,
 *  "in_reply_to_user_id_str": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet的使用者ID（以字串表示）,
 *  "lang": 根據機器偵測自動判斷出該Tweet的語言,
 *  "created_at": 使用者發出Tweet的時間,
 *  "in_reply_to_status_id_str": 可為空值，若這篇Tweet為回覆別人的Tweet，會顯示原Tweet的使用者ID（以字串表示）,
 *  "place": 該Tweet是否有與某地連結,
 *  "metadata": 
    * "iso_language_code": 該網站使用的語系,
    * "result_type": Tweet的型態為何，是熱門Tweet還是近期所發出的Tweet
```
