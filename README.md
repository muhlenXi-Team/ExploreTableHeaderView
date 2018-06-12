# ExploreTableHeaderView
About tableHeaderView

示例代码：

```swift
if (@available(iOS 11.0, *)) {
    [self.tableView performBatchUpdates:^{
        self.tableView.tableHeaderView  = self.headerView;
    } completion:^(BOOL finished) {
    }];
} else {
    [self.tableView beginUpdates];
    self.tableView.tableHeaderView  = self.headerView;
    [self.tableView endUpdates];
}
```



