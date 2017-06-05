

# 隐藏滑动条

```
mCollectionView?.showsHorizontalScrollIndicator = false
mCollectionView?.showsVerticalScrollIndicator = false
```

# 设置 cell 大小充满 UICollectioinView

```
    func collectionView(_ collectionView: UICollectionView,
                        layout collectionViewLayout: UICollectionViewLayout,
                        sizeForItemAt indexPath: IndexPath) -> CGSize {
        return collectionView.frame.size
    }
```

# 监听滑动

```
    func scrollViewDidScroll(_ scrollView: UIScrollView) {
        // offset: mCollectionView?.contentOffset.y        
    }
```