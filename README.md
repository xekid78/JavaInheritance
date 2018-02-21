# JavaInheritance
継承

## 処理
Boxクラスを親クラスとしてJewelryBoxクラスを子クラスにして処理を行う。

## コード
```
public class Sample31 {

	public static void main(String[] args) {
		Box box = new Box();
		box.open();

		JewelryBox jewelrybox = new JewelryBox();
		jewelrybox.look();
		jewelrybox.open();

	}

}

class Box {
	public String myItem;

	public Box() {
		myItem = "新しいアイテム";
	}

	public void open() {
		System.out.println("宝箱を開いた。" + myItem + "を手に入れた。");
	}
}

class JewelryBox extends Box {
	public void look() {
		System.out.println("宝箱はキラキラと輝いている");
	}
}
```

## 出力結果  
```
宝箱を開いた。新しいアイテムを手に入れた。
宝箱はキラキラと輝いている
宝箱を開いた。新しいアイテムを手に入れた。
```
  
## 開発環境
| 開発ツール |  |
|:-|:-|
| 統合開発環境(IDE) | Eclipse 4.7.0 Oxygen |
| 開発言語 | Java8 |
