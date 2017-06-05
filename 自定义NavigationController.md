
2017/5/19

# Install


# 设置成透明

```
    override func viewWillAppear(_ animated: Bool) {
        super.viewWillAppear(animated)
        self.navigationController?.navigationBar.setBackgroundImage(UIImage(), for: UIBarMetrics.default)
        self.navigationController?.navigationBar.shadowImage = UIImage()
    }
    
    override func viewWillDisappear(_ animated: Bool) {
        super.viewWillDisappear(animated)
        self.navigationController?.navigationBar.shadowImage = nil
        self.navigationController?.navigationBar.setBackgroundImage(nil, for: UIBarMetrics.default)
    }
```