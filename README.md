# PINKBindView

[![Version](https://img.shields.io/cocoapods/v/PINKBindView.svg?style=flat)](http://cocoadocs.org/docsets/PINKBindView)
[![License](https://img.shields.io/cocoapods/l/PINKBindView.svg?style=flat)](http://cocoadocs.org/docsets/PINKBindView)
[![Platform](https://img.shields.io/cocoapods/p/PINKBindView.svg?style=flat)](http://cocoadocs.org/docsets/PINKBindView)


PINKBindView provide a simple way to use tableView and collectionView.

## Usage

Such as
```objc
[self.tableView setDataSourceSignal:RACObserve(self, list)
              	   selectionCommand:self.selectionCommand
                    		cellNib:CustomTableViewCell.viewNib];
```
And you should implementation this method in your cell class:
```objc
- (void)bindCellViewModel:(id)viewModel indexPath:(NSIndexPath *)indexPath
```            						
You also can run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

iOS 6+

## Installation

PINKBindView is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

    pod "PINKBindView"

## License

PINKBindView is available under the MIT license. See the LICENSE file for more info.

