## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能 https://zipcloud.ibsnet.co.jp/api/search 郵便番号に対してそれに関連する住所の情報を表示する
* リクエストとレスポンスのフォーマット リクエスト{
	"message": "必須パラメータが指定されていません。",
	"results": null,
	"status": 400
}

レスポンスのフォーマット
{
	"message": null,
	"results": [
		{
			"address1": "北海道",
			"address2": "美唄市",
			"address3": "上美唄町協和",
			"kana1": "ﾎｯｶｲﾄﾞｳ",
			"kana2": "ﾋﾞﾊﾞｲｼ",
			"kana3": "ｶﾐﾋﾞﾊﾞｲﾁｮｳｷｮｳﾜ",
			"prefcode": "1",
			"zipcode": "0790177"
		},
		{
			"address1": "北海道",
			"address2": "美唄市",
			"address3": "上美唄町南",
			"kana1": "ﾎｯｶｲﾄﾞｳ",
			"kana2": "ﾋﾞﾊﾞｲｼ",
			"kana3": "ｶﾐﾋﾞﾊﾞｲﾁｮｳﾐﾅﾐ",
			"prefcode": "1",
			"zipcode": "0790177"
		}
	],
	"status": 200
}
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL The Cat API https://thecatapi.com/
* エンドポイントと機能 https://api.thecatapi.com/v1/images/search 猫のランダムな画像を表示する
* リクエストとレスポンスのフォーマット リクエスト {
  "id": "0XYvRd7oD",
  "url": "https://cdn2.thecatapi.com/images/0XYvRd7oD.jpg",
  "breeds": [
    {
      "weight": {
        "imperial": "7  -  10",
        "metric": "3 - 5"
      },
      "id": "abys",
      "name": "Abyssinian",
      "cfa_url": "http://cfa.org/Breeds/BreedsAB/Abyssinian.aspx",
      "vetstreet_url": "http://www.vetstreet.com/cats/abyssinian",
      "vcahospitals_url": "https://vcahospitals.com/know-your-pet/cat-breeds/abyssinian",
      "temperament": "Active, Energetic, Independent, Intelligent, Gentle",
      "origin": "Egypt",
      "country_codes": "EG",
      "country_code": "EG",
      "description": "The Abyssinian is easy to care for, and a joy to have in your home. They’re affectionate cats and love both people and other animals.",
      "life_span": "14 - 15",
      "indoor": 0,
      "lap": 1,
      "alt_names": "",
      "adaptability": 5,
      "affection_level": 5,
      "child_friendly": 3,
      "dog_friendly": 4,
      "energy_level": 5,
      "grooming": 1,
      "health_issues": 2,
      "intelligence": 5,
      "shedding_level": 2,
      "social_needs": 5,
      "stranger_friendly": 5,
      "vocalisation": 1,
      "experimental": 0,
      "hairless": 0,
      "natural": 1,
      "rare": 0,
      "rex": 0,
      "suppressed_tail": 0,
      "short_legs": 0,
      "wikipedia_url": "https://en.wikipedia.org/wiki/Abyssinian_(cat)",
      "hypoallergenic": 0,
      "reference_image_id": "0XYvRd7oD"
    }
  ],
  "width": 1204,
  "height": 1445
}

レスポンスのフォーマット
[{
"id":"ebv",
"url":"https://cdn2.thecatapi.com/images/ebv.jpg",
"width":176,"height":540,
"breeds":[],
"favourite":{}
}]
### Q3-3. 感想
* 今回の課題で苦労したこと 使用するAPIを探すこと 呼び出しと表示のコード記入
* 演習を通して理解できたこと 外部APIの呼び出しの方法 WebAPIの仕組みと構成要素
* Web APIの利便性や課題など 利便性:Webブラウザから直接アクセスできる手軽さ Web経由であるため常に最新の情報を取得できる 汎用性の高さ 
課題:提供元に依存してしまうこと セキュリティ安全性の低さ サービスによっては費用がかさむ可能性あり





