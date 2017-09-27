Forked from @topdown's [VVV Dashboard](https://github.com/topdown/VVV-Dashboard) - fixed for VVV2

Setup
-
Clone this repo to your VVV/www/default/ directory and then copy dashboard-custom.php there:

```
cd www/default
git clone https://github.com/khleomix/VVV-Dash.git dashboard
cp dashboard/dashboard-custom.php .
```

While VVV is running (`vagrant up`), the new dashboard is now viewable at your VVV root (usually [vvv](http://vvv) or [vvv.dev](http://vvv.dev)).

Update
-
Update your repo via `git pull` and then copy dashboard-custom.php to your default directory.
```
cd www/default/dashboard
git pull
cp dashboard-custom.php ..
```

Note
-
If sites are not created, check if you have the `vvv-hosts` file inside the `provision` directory. If none, create a `vvv-hosts` with the following content:

`yoursite.dev`

---


### Change Log

---

mm/dd/yy

09/27/17 version: 0.2.0.2
* Fix README with additional instructions to make it work with VVV2

09/25/17 version: 0.2.0.1

* Added hotfix to load provisioned domains as per https://github.com/topdown/VVV-Dashboard/issues/52#issuecomment-322917895

