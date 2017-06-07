
2017/6/6



# 


```
dataSource.configureCell = { (ds: RxTableViewSectionedReloadDataSource<SectionOfCustomData>, tv: UITableView, ip: IndexPath, item: Item) in
  let cell = tv.dequeueReusableCell(withIdentifier: "Cell", for: ip)
  cell.textLabel?.text = "Item \(item.anInt): \(item.aString) - \(item.aCGPoint.x):\(item.aCGPoint.y)"
  return cell
}
```



# itemSelected

点击事件

```
mTableView.rx.itemSelected.subscribe(onNext:{ indexPath in
    let model = self.mVM.mDataSource.value[indexPath.row]
    self.navigationController?.pushViewController(CourseDetailVC(courseId: model.termCourseId!, courseName: model.termCourseName!), animated: true)
            
}).disposed(by: mDisposeBag)
```        





