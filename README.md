# Django Inventory Management App

This is a small, focused Django inventory-management app that demonstrates a complete CRUD workflow for products using **function-based views** and **ModelForms**. It’s a learning/portfolio project to show how to **model data**, **build forms**, and wire up basic **create/read/update/delete** flows in Django. 

## About
This repo is an adaptation of [Complete Django Tutorial](https://www.youtube.com/playlist?list=PL4cUxeGkcC9iqfAag3a_BKEX1N43uJutw) by Bek Brace. 

I followed the tutorial to learn followings:
* Create an app that manages `Product` records (create, list/read, update, delete).
* Implement a `Product` model with these fields: `product_id` (AutoField primary key), `name`, `sku` (unique), `price`, `quantity`, and `supplier`.
* Implement a `ProductForm` (`ModelForm`) with Bootstrap-ready widgets and helpful placeholders for each field.
* Implement function-based views:
  * `home_view` — index page.
  * `product_create_view` — add product (POST → save → redirect).
  * `prouct_list_view` — show all products.
  * `product_update_view` — edit an existing product (by `product_id`).
  * `product_delete_view` — confirm & delete.
* URL patterns map to the views (`''`, `create/`, `list/`, `update/<int:product_id>/`, `delete/<int:product_id>/`).
* Templates: `invApp/home.html`, `invApp/product_form.html`, `invApp/product_list.html`, `invApp/product_confirm_delete.html`, `layout.html`.

**Why this project is useful**
* Shows practical use of Django `models`, `forms.ModelForm`, and `views` to implement real features.
* Demonstrates server-side form handling, validation *(e.g., unique SKU enforced at the model level)*, and clean redirects after POSTs.
* Widgets include Bootstrap classes so the UI can be styled quickly with Bootstrap for a polished look.


## How to run (dev)
1. `git clone https://github.com/webQbe/dj5_invproject.git`
2. `python -m venv .venv && source .venv/bin/activate`
3. `pip install -r requirements.txt`
4. `python manage.py migrate && python manage.py createsuperuser`
5. `python manage.py runserver`
---
Then open your browser and go to:
👉 **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**


## Credits
Original tutorial: [Complete Django Tutorial](https://www.youtube.com/playlist?list=PL4cUxeGkcC9iqfAag3a_BKEX1N43uJutw) — Net Ninja

## License
MIT License






