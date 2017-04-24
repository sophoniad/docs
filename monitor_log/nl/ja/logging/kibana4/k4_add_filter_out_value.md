---

copyright:
  years: 2015, 2017

lastupdated: "2017-03-01"

---


{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:screen: .screen}

# *フィールド・リスト* でリストされない値のフィルターの追加
{:#k4_add_filter_out_value}

*フィールド・リスト* に表示されていない値のフィルターを追加するには、照会を介してその値が含まれているレコードを検索します。その後、「Discover」ページで使用可能な表項目からフィルターを追加します。
{:shortdesc}

*フィールド・リスト*・セクションに表示されるリストで使用可能でない値のフィルターを追加するには、以下のステップを実行します。

1. Kibana の「Discover」ページを見て、表示されているデータのサブセットを確認します。詳しくは、『[「Discover」ページで表示されているデータの識別](logging_kibana_analize_logs_interactively.html#k4_identify_data)』を参照してください。

    例えば、以下の図では、*フィールド・リスト* 内の CF アプリのインスタンスの値を示しています。 
    
    ![フィールド・リストでの値を表示](images/k4_add_filter_f1.jpg "フィールド・リストでの値を表示")
    
    インスタンス番号 *3* に関心があるのにもかかわらず、表示されるリストでそのインスタンスが使用可能でありません。

2. 「Discover」ページで、特定のフィールド値を検索するように照会を変更します。

    例えば、インスタンス *3* を検索する場合、入力する照会は以下のようになります。
   `application_id:9d222152-8834-4bab-8685-3036cd25931a AND instance_id:"3"`
    
    ![照会の変更](images/k4_add_filter_f2.jpg "照会の変更")
    
    表で、照会に一致したすべてのレコードが表示されます。 
    
 3. 1 つのレコードを展開し、拡大鏡ボタン ![拡大鏡ボタン (包含モード)](images/k4_include_field_icon.jpg "拡大鏡ボタン (包含)") を選択してフィルターを追加します。
 
     例えば、値が *3* のインスタンス ID のフィルターを追加するには、*instance_id* フィールドの横にある拡大鏡ボタン ![拡大鏡ボタン (包含モード)](images/k4_include_field_icon.jpg "拡大鏡ボタン (包含)") をクリックします。
     
     ![表の表示](images/k4_add_filter_f3.jpg "表の表示")
     
4. フィルターが追加されたことを確認します。

    例えば、以下の表では、表からフィルターを追加した後に有効になっているフィルターを示しています。
    
    ![フィルターの表示](images/k4_add_filter_f4.jpg "フィルターの表示")
    
    