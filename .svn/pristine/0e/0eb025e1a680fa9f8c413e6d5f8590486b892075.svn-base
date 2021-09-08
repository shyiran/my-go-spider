package main

import (
	"fmt"
	"my-go-spider/gofish"
	"my-go-spider/handle"
)

func main() {
	authors := "https://so.gushiwen.org/authors/"
	h := handle.AuthorHandle{}
	fish := gofish.NewGoFish()
	request, err := gofish.NewRequest("GET", authors, gofish.UserAgent, &h, nil)
	if err != nil {
		fmt.Println(err)
		return
	}
	fish.Request = request
	fish.Visit()
	//res, err := http.Get(authors)
	//if err != nil {
	//	fmt.Println("读取网页信息失败！")
	//}
	//defer res.Body.Close()
	//if res.StatusCode != 200 {
	//	log.Fatalf("status code err %d,%s", res.StatusCode, res.Status)
	//}
	//doc, err := goquery.NewDocumentFromReader(res.Body)
	//if err != nil {
	//	fmt.Errorf(" doc err")
	//}
	//doc.Find(".sons").Find(".cont").Find("a").Each(func(i int, selection *goquery.Selection) {
	//	author := selection.Text()
	//	fmt.Printf("%d author %s\n", i, author)
	//	link, _ := selection.Attr("href")
	//	fmt.Printf("%d link=%s\n", i, link)
	//})

	//
	//
	//
	//	if err!=nil{
	//		fmt.Println(err)
	//		return
	//	}
	//	fish.Request = request
	//
}
