Глобальные переменные Smarty в шаблонах PrestaShop 1.7
============

Действующие глобальные переменные
-------

| Command | Description |
| --- | --- |
| --- | **Админка** |
| **{$urls\|@var_dump}** | -> Содержит Prestashop urls; |
| **{$urls.base_url}** | Базовый url магазина в виде http://bookattic.ru/; |
| **{$urls.current_url}** | Текущий url магазина в виде http://bookattic.ru/; |
| --- | --- |
| **{$shop\|@var_dump}** | -> Содержит данные магазина (название, email, телефон, прочее...); |
| **{$shop.name}** | Имя магазина; |
| **{$shop.email}** | E-mail магазина; |
| **{$shop.logo}** | Логотип магазина в виде /img/logo.jpg; |
| **{$shop.stores_icon}** | Изображение магазина в виде /img/logo_stores.png; |
| **{$shop.favicon}** | Иконка магазина в виде /img/favicon.ico; |
| **{$shop.phone}** | Телефон магазина; |
| **{$shop.fax}** | Факс магазина; |
| **{$shop.address.formatted}** | Форматированный адрес магазина в виде Bookattic<br>Днепропетровская ул.<br>Москва<br>Russian Federation; |
| **{$shop.address.address1}** | Адрес 1 магазина; |
| **{$shop.address.address2}** | Адрес 2 магазина; |
| **{$shop.address.postcode}** | Почтовый индекс магазина; |
| **{$shop.address.city}** | Город магазина; |
| **{$shop.address.state}** | Штат, область магазина; |
| **{$shop.address.country}** | Страна магазина; |
| --- | --- |
| **{$page\|@var_dump}** | -> Содержит данные текущей страницы; |
| **{$page.title}** | Заглавие страницы; |
| **{$page.description}** | Описание страницы; |
| **{$page.keywords}** | Ключевые слова страницы; |
| **{$page.robots}** | Роботс страницы; |
| **{$page.page_name}** | Название страницы; |
| --- | --- |
| **{$currency\|@var_dump}** | -> Currency variables; |
| **{$language\|@var_dump}** | -> Language variables; |
| **{$customer\|@var_dump}** | -> Customer variables; |
| **{$configuration\|@var_dump}** | -> Configuration variables; |
| --- | --- |
| **{$link\|@var_dump}** | -> Link variables; |
| --- | --- |
| **{$breadcrumb\|@var_dump}** | -> Breadcrumb variables; |
| --- | --- |
| --- | **And here are some ready-tu-use variables:** |
| --- | --- |
| **{$currency.name}** | -> Name of the active currency.  |
| **{$currency.iso_code}** | -> ISO language code enabled.  |
| **{$currency.sign}** | -> Symbol of the active currency  |
| **{$currency.iso_code_num}** | -> Active Currency ISO Code |
| --- | --- |
| **{$shop.name}** | -> Store name in Prestashop 1.7  |
| **{$shop.email}** | -> Store Email in Prestashop 1.7  |
| **{$shop.logo}** | -> Image routing store logo in Prestashop 1.7  |
| **{$shop.favicon}** | -> Route favicon image of the store in Prestashop 1.7  |
| **{$shop.address.address1}** | -> Store address 1 in Prestashop 1.7  |
| **{$shop.address.address2}** | -> Store address 2 in Prestashop 1.7  |
| **{$shop.address.postcode}** | -> Store Zip Code in Prestashop 1.7  |
| **{$shop.address.city}** | -> Store City in Prestashop 1.7  |
| **{$shop.address.state}** | -> Province of the store in Prestashop 1.7  |
| **{$shop.address.country}** | -> Shop Country in Prestashop 1.7  |
| **{$shop.phone}** | -> Store phone in Prestashop 1.7  |
| **{$shop.fax}** | -> Store Fax in Prestashop 1.7 |
| --- | --- |
| **{$language.name}** | -> Language name enabled  |
| **{$language.iso_code}** | -> ISO language code enabled  |
| **{$language.language_code}** | -> Language code enabled (for Spanish, fr for French, tc ..)  |
| **{$language.is_rtl}** | -> (1 -> On / 0 Off (for when language is written from right to left)  |
| **{$language.format_lite}** | and {$ language.format_full} -> Simulated date format and full date format  |
| **{$language.id}** | -> Language ID enabled |
| --- | --- |
| **{$customer.lastname}** | -> Customer Last Name in Prestashop 1.7 |
| **{$customer.firstname}** | -> Client Name Prestashop 1.7 |
| **{$customer.email}** | -> Prestashop Customer Email 1.7 |
| **{$customer.birthday}** | -> Prestashop client birthday 1.7 |
| **{$customer.newsletter}** | -> Subscribed to the newsletter in Prestashop 1.7 (1 subscribed / 0 unsubscribed) |
| **{$customer.newsletter_date_add}** | -> Newsletter subscription date |
| **{$customer.ip_registration_newsletter}** | -> IP Registration Customers newsletter |
| **{$customer.optin}** | -> Subscribed to offers from our partners in Prestashop 1.7  |
| **{$customer.date_add}** | -> Client creation date in Prestashop 1.7 |
| **{$customer.date_upd}** | -> Last updated client update in Prestashop 1.7 |
| **{$customer.id}** | -> Customer ID in Prestashop 1.7 |
| **{$customer.id_default_group}** | -> Default group to which the client is associated in Prestashop 1.7 |
| **{$customer.is_logged}** | -> Check if the client is "logged in" in Prestashop 1.7 |
| **{$customer.gender.name [$ customer.gender.id]}** | -> Client Gender (Mr / Ms) |
| **{$customer.addresses [Address ID] .city}** | -> Client city of address 'X' that has partner. (Address ID, because a client can theoretically have multiple addresses) |
| **{$customer.addresses [Address ID] .alias}** | -> Address alias |
| **{$customer.addresses [Address ID] .firstname}** | -> Addressholder last name |
| **{$customer.addresses [Address ID] .lastname}** | -> Name of address holder |
| **{$customer.addresses [Address ID] .company}** | -> Company name of address holder |
| **{$customer.addresses [Address ID] .address1}** | -> Address 1 |
| **{$customer.addresses [Address ID] .address2}** | -> Address 2 |
| **{$customer.addresses [Address ID] .postcode}** | -> Mailing address |
| **{$customer.addresses [Address ID] .id_state}** | -> Address Province ID |
| **{$customer.addresses [Address ID] .state}** | -> Province address |
| **{$customer.addresses [Address ID] .state_iso}** | -> ISO address province code |
| **{$customer.addresses [Address ID] .id_country}** | -> Country address ID |
| **{$customer.addresses [Address ID] .country}** | -> Country of address |
| **{$customer.addresses [Address ID] .country_iso}** | -> ISO country address code |
| **{$customer.addresses [Address ID] .phone}** | -> Address phone |
| **{$customer.addresses [Address ID] .phone_mobile}** | -> Mobile phone address |
| **{$customer.addresses [iD Address] .dni}** | -> Address ID |
| **{$customer.addresses [Address ID] .vat_number}** | -> Customer VAT number |
| **{$customer.addresses [Address ID] .formatted}** | -> Client formatted address |
| --- | --- |
| **{$urls.base_url}** | -> Store address  |
| **{$urls.current_url}** | -> Current address (url) where we are  |
| **{$urls.shop_domain_url}** | -> Store domain  |
| **{$urls.img_ps_url}** | -> Image root directory url  |
| **{$urls.img_cat_url}** | -> Url directory of images of the categories  |
| **{$urls.img_lang_url}** | -> Url of the language images directory  |
| **{$urls.img_prod_url}** | -> Url of the product images directory  |
| **{$urls.img_manu_url}** | -> Url directory of manufacturers images  |
| **{$urls.img_sup_url}** | -> Url of the providers directory  |
| **{$urls.img_ship_url}** | -> Url directory of images of carriers  |
| **{$urls.img_store_url}** | -> Store url |
| **{$urls.img_url}** | -> Url of the image directory of the template  |
| **{$urls.css_url}** | -> Template URL directory url  |
| **{$urls.js_url}** | -> Template JS directory url  |
| **{$urls.pic_url}** | -> Url file directory uploaded  |
| **{$urls.pages.address}** | -> Url from the "My Address" section  |
| **{$urls.pages.addresses}** | -> Url from the "My addresses" section  |
| **{$urls.pages.authentication}** | -> Url section of the authentication page  |
| **{$urls.pages.cart}** | -> Cart section url (order summary)  |
| **{$urls.pages.category}** | -> Url section of categories  |
| **{$urls.pages.cms}** | -> Url of the content section  |
| **{$urls.pages.contact}** | - > Url section of the contact form  |
| **{$urls.pages.discount}** | -> Url of the discount voucher section  |
| **{$urls.pages.guest_tracking}** | -> Tracking url for unregistered clients  |
| **{$urls.pages.history}** | -> Url from the order history section  |
| **{$urls.pages.identity}** | -> Url of the section "Personal data"  |
| **{$urls.pages.index}** | -> Page url  |
| **{$urls.pages.my_account}** | -> Url section of my account  |
| **{$urls.pages.order_confirmation}** | -> Url section of the order confirmation page.  |
| **{$urls.pages.order_follow}** | - > Url in the "Order Tracking"  |
| **{$urls.pages.order}** | -> Url of the order page |
| **{$urls.pages.order_return}** | -> Url of the order return page |
| **{$urls.pages.order_slip}** | -> Url of the order slip page |
| **{$urls.pages.pagenotfound}** | -> Url of section "404 (Page not found)"  |
| **{$urls.pages.password}** | -> Url of the section "Recover Password"  |
| **{$urls.pages.pdf_invoice}** | -> Pdf invoice page url |
| **{$urls.pages.pdf_order_return}** | -> Pdf order return page url |
| **{$urls.pages.pdf_order_slip}** | -> Pdf order slip url page |
| **{$urls.pages.prices_drop}** | -> Url section we lowered prices / products discount / discounts  |
| **{$urls.pages.product}** | -> Product tab url  |
| **{$urls.pages.search}** | -> Url of the searcher section  |
| **{$urls.pages.sitemap}** | -> Site Map section url  |
| **{$urls.pages.stores}** | -> Url of the section "Shops / Our stores"  |
| **{$urls.pages.supplier}** | -> Url from the providers section  |
| **{$urls.pages.register}** | -> Url log page  |
| **{$urls.pages.order_login}** | -> Order login page url |
| **{$urls.theme_assets}** | -> Url of the "assets" directory of the template / themes / template / assets /  |
| **{$urls.actions.logout}** | -> Url to close section in the store |


