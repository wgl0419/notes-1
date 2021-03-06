- [iOS 开发随手记](#ios-%e5%bc%80%e5%8f%91%e9%9a%8f%e6%89%8b%e8%ae%b0)
  - [多 target](#%e5%a4%9a-target)
  - [加快编译速度](#%e5%8a%a0%e5%bf%ab%e7%bc%96%e8%af%91%e9%80%9f%e5%ba%a6)
  - [扩大 button 响应区域](#%e6%89%a9%e5%a4%a7-button-%e5%93%8d%e5%ba%94%e5%8c%ba%e5%9f%9f)
  - [UILabel 文本靠左上角](#uilabel-%e6%96%87%e6%9c%ac%e9%9d%a0%e5%b7%a6%e4%b8%8a%e8%a7%92)
  - [UILabel 设置行间隙](#uilabel-%e8%ae%be%e7%bd%ae%e8%a1%8c%e9%97%b4%e9%9a%99)
  - [去除 String 中的空格](#%e5%8e%bb%e9%99%a4-string-%e4%b8%ad%e7%9a%84%e7%a9%ba%e6%a0%bc)
  - [UILabel 部分文字可点击](#uilabel-%e9%83%a8%e5%88%86%e6%96%87%e5%ad%97%e5%8f%af%e7%82%b9%e5%87%bb)
  - [找到所有 subviewClass 类](#%e6%89%be%e5%88%b0%e6%89%80%e6%9c%89-subviewclass-%e7%b1%bb)
  - [找到 subviewClass 这个类的父视图](#%e6%89%be%e5%88%b0-subviewclass-%e8%bf%99%e4%b8%aa%e7%b1%bb%e7%9a%84%e7%88%b6%e8%a7%86%e5%9b%be)
  - [iOS13 适配](#ios13-%e9%80%82%e9%85%8d)
  - [RAC 通知的移除](#rac-%e9%80%9a%e7%9f%a5%e7%9a%84%e7%a7%bb%e9%99%a4)
  - [类方法里使用 self](#%e7%b1%bb%e6%96%b9%e6%b3%95%e9%87%8c%e4%bd%bf%e7%94%a8-self)
  - [拍照后修复图片方向 `fixOrientation` & 剪切图片 `imageByCroppingWithRect`](#%e6%8b%8d%e7%85%a7%e5%90%8e%e4%bf%ae%e5%a4%8d%e5%9b%be%e7%89%87%e6%96%b9%e5%90%91-fixorientation--%e5%89%aa%e5%88%87%e5%9b%be%e7%89%87-imagebycroppingwithrect)
  - [设置APP支持的文件类型 eg:PDF](#%e8%ae%be%e7%bd%aeapp%e6%94%af%e6%8c%81%e7%9a%84%e6%96%87%e4%bb%b6%e7%b1%bb%e5%9e%8b-egpdf)
  - [`Bundle.main.paths(forResourcesOfType: "pdf", inDirectory: "swift_lang")` 方法获取不到文件解决](#bundlemainpathsforresourcesoftype-%22pdf%22-indirectory-%22swiftlang%22-%e6%96%b9%e6%b3%95%e8%8e%b7%e5%8f%96%e4%b8%8d%e5%88%b0%e6%96%87%e4%bb%b6%e8%a7%a3%e5%86%b3)
  - [Xcode11 新建项目，去除 SceneDelegate.swift](#xcode11-%e6%96%b0%e5%bb%ba%e9%a1%b9%e7%9b%ae%e5%8e%bb%e9%99%a4-scenedelegateswift)
  - [Xcode 报错](#xcode-%e6%8a%a5%e9%94%99)
  - [旋转动画](#%e6%97%8b%e8%bd%ac%e5%8a%a8%e7%94%bb)
  - [方法废弃](#%e6%96%b9%e6%b3%95%e5%ba%9f%e5%bc%83)
  - [NSURL 的 query 、path 等方法](#nsurl-%e7%9a%84-query-path-%e7%ad%89%e6%96%b9%e6%b3%95)
  - [修改 UIPickerView 中的文字大小](#%e4%bf%ae%e6%94%b9-uipickerview-%e4%b8%ad%e7%9a%84%e6%96%87%e5%ad%97%e5%a4%a7%e5%b0%8f)
  - [深拷贝](#%e6%b7%b1%e6%8b%b7%e8%b4%9d)
  - [[Application] The app delegate must implement the window property if it wants to use a main storyboard file.](#application-the-app-delegate-must-implement-the-window-property-if-it-wants-to-use-a-main-storyboard-file)
  - [秒数转成 00:00:00 格式  eg: 60s -> 00:01:00](#%e7%a7%92%e6%95%b0%e8%bd%ac%e6%88%90-000000-%e6%a0%bc%e5%bc%8f-eg-60s---000100)
  - [添加 pch 文件时候路径怎么写](#%e6%b7%bb%e5%8a%a0-pch-%e6%96%87%e4%bb%b6%e6%97%b6%e5%80%99%e8%b7%af%e5%be%84%e6%80%8e%e4%b9%88%e5%86%99)
  - [iOS 添加点击效果，方便录屏时候看触点](#ios-%e6%b7%bb%e5%8a%a0%e7%82%b9%e5%87%bb%e6%95%88%e6%9e%9c%e6%96%b9%e4%be%bf%e5%bd%95%e5%b1%8f%e6%97%b6%e5%80%99%e7%9c%8b%e8%a7%a6%e7%82%b9)
  - [model类转字典](#model%e7%b1%bb%e8%bd%ac%e5%ad%97%e5%85%b8)
  - [iOS10上的 navgaitionBarItem 不显示问题](#ios10%e4%b8%8a%e7%9a%84-navgaitionbaritem-%e4%b8%8d%e6%98%be%e7%a4%ba%e9%97%ae%e9%a2%98)
  - [class_copyPropertyList 不能复制父类的属性](#classcopypropertylist-%e4%b8%8d%e8%83%bd%e5%a4%8d%e5%88%b6%e7%88%b6%e7%b1%bb%e7%9a%84%e5%b1%9e%e6%80%a7)
  - [git 报错：refusing to merge unrelated histories](#git-%e6%8a%a5%e9%94%99refusing-to-merge-unrelated-histories)
  - [字符串某些变色](#%e5%ad%97%e7%ac%a6%e4%b8%b2%e6%9f%90%e4%ba%9b%e5%8f%98%e8%89%b2)
  - [编译不过，storyboard 报错 : internal error.](#%e7%bc%96%e8%af%91%e4%b8%8d%e8%bf%87storyboard-%e6%8a%a5%e9%94%99--internal-error)
  - [UITableView haader 悬浮效果](#uitableview-haader-%e6%82%ac%e6%b5%ae%e6%95%88%e6%9e%9c)
  - [让 UITableViewController 的 tableview 内容在状态栏下](#%e8%ae%a9-uitableviewcontroller-%e7%9a%84-tableview-%e5%86%85%e5%ae%b9%e5%9c%a8%e7%8a%b6%e6%80%81%e6%a0%8f%e4%b8%8b)
  - [关闭 iOS13 的黑暗模式](#%e5%85%b3%e9%97%ad-ios13-%e7%9a%84%e9%bb%91%e6%9a%97%e6%a8%a1%e5%bc%8f)
  - [贝塞尔曲线添加阴影](#%e8%b4%9d%e5%a1%9e%e5%b0%94%e6%9b%b2%e7%ba%bf%e6%b7%bb%e5%8a%a0%e9%98%b4%e5%bd%b1)
  - [两个角切圆角](#%e4%b8%a4%e4%b8%aa%e8%a7%92%e5%88%87%e5%9c%86%e8%a7%92)
  - [修改UIAlertAction文字颜色](#%e4%bf%ae%e6%94%b9uialertaction%e6%96%87%e5%ad%97%e9%a2%9c%e8%89%b2)
  - [设置 UITextField 和 UIDatePicker 联动](#%e8%ae%be%e7%bd%ae-uitextfield-%e5%92%8c-uidatepicker-%e8%81%94%e5%8a%a8)
  - [使用 CoreLocation 定位](#%e4%bd%bf%e7%94%a8-corelocation-%e5%ae%9a%e4%bd%8d)
- [xib & storyboard](#xib--storyboard)
  - [xib 创建 UIView](#xib-%e5%88%9b%e5%bb%ba-uiview)
  - [获取故事版上的vc](#%e8%8e%b7%e5%8f%96%e6%95%85%e4%ba%8b%e7%89%88%e4%b8%8a%e7%9a%84vc)
  - [UITableViewController 静态 cell 和动态 cell 混用](#uitableviewcontroller-%e9%9d%99%e6%80%81-cell-%e5%92%8c%e5%8a%a8%e6%80%81-cell-%e6%b7%b7%e7%94%a8)
  - [让自定义 view 在 xib 或 storyboard 上也能用](#%e8%ae%a9%e8%87%aa%e5%ae%9a%e4%b9%89-view-%e5%9c%a8-xib-%e6%88%96-storyboard-%e4%b8%8a%e4%b9%9f%e8%83%bd%e7%94%a8)

# iOS 开发随手记 

- [iOS开发随手记 - 简书](https://www.jianshu.com/p/cb80ad438057)
## 多 target

 >  BWCMT 项目架构:
 >
 >  - 基础库 pod 集成（封装好的 UI；网络库；三方库等）
 >  - 每个业务线是一个 project，最后主工程依赖各个业务线 framework，业务线间通信通过平台层platform 里的路由完成（不能跨业务线直接调用）
 >
 >  ![bwcmt_struct](../../src/imgs/ios/bwcmt_struct.png)
 >
 >  产生的问题：主工程依赖所有的业务线的framework，但是各个业务线之间不一定有依赖，我开发某一个业务线的时候，如果需要编译整个工程的话，时间会很长。
 >
 >  解决方案是：为一个单独的业务线创建一个target，以节省工程build时间。


**创建多 target 方法**

  创建target的步骤参考这个链接：[iOS 一套代码多APP／多渠道／多target+自动打包脚本](https://www.jianshu.com/p/73343b4fc42b)

  [创建多target](./add_more_targets_to_your_project.md)

**创建一个新 target 的注意点：**

  + 依赖
    
    ![more_targets_noti0](../../src/imgs/ios/more_targets_noti0.png)
  + 宏：判断当前run的那个target
  
    ![more_targets_noti1](../../src/imgs/ios/more_targets_noti1.png)
    ![more_targets_noti2](../../src/imgs/ios/more_targets_noti2.png)

    设置`$(inherited)`

    ![more_target_error_pod_solve](../../src/imgs/ios/more_target_error_pod_solve.png)
  + Pods库：新的target也要记得依赖pod库

    ```ruby
      # Podfile 文件
      targetsArray = ['BWCMTApp','BWCMTAppYZFlutter']

      targetsArray.each  do |t|

         target t do
             pod 'YYModel', '~>1.0.4'
             pod 'DoraemonKit/Core', :git => 'http://gitlab.10101111.com:8888/p2p/udoraemonkit.git', :configurations => ['Debug','ZC','Distribution']
         end
      end
    ```

**多 target 设置 `GCC_PREPROCESSOR_DEFINITIONS` 引起的问题**

前面说了，为了用代码判断当前run的是那个target，设置了两个宏`BWCMT_FULL`和`BWCMT_YZ_FLUTTER`。这时候使用`pod install`会有下面的提示（pod没有出错，只是会给个警告⚠️）。

  ```shell
    [!] The `BWCMTApp [Release]` target overrides the `GCC_PREPROCESSOR_DEFINITIONS` build setting defined in `Pods/Target Support Files/Pods-BWCMTApp/Pods-BWCMTApp.release.xcconfig'. This can lead to problems with the CocoaPods installation
     - Use the `$(inherited)` flag, or
     - Remove the build settings from the target.
  ```

   ![more_target_error_pod](../../src/imgs/ios/more_target_error_pod.png)

   解决办法是在`GCC_PREPROCESSOR_DEFINITIONS`里加上`$(inherited)`。再次`pod install`警告会消失。

   ![more_target_error_pod_solve](../../src/imgs/ios/more_target_error_pod_solve.png)

## 加快编译速度

从源码到二进制可执行文件整个流程去考虑

1. 修改`Optimization Level`的值

    ![Optimization Level](../../src/imgs/ios/optimization_level.png)

2. `.h`文件引入头文件，`#import`改成`@class`



## 扩大 button 响应区域

```objc
/// .h

@interface UIButton (EnlargeHitArea)

@property (nonatomic, assign) UIEdgeInsets hitTestEdgeInsets;

@end

/// .m

#import "UIButton+EnlargeHitArea.h"
static const NSString *KEY_HIT_TEST_EDGE_INSETS = @"HitTestEdgeInsets";

@implementation UIButton (EnlargeHitArea)

-(void)setHitTestEdgeInsets:(UIEdgeInsets)hitTestEdgeInsets {
    NSValue *value = [NSValue value:&hitTestEdgeInsets withObjCType:@encode(UIEdgeInsets)];
    objc_setAssociatedObject(self, &KEY_HIT_TEST_EDGE_INSETS, value, OBJC_ASSOCIATION_RETAIN_NONATOMIC);
}

-(UIEdgeInsets)hitTestEdgeInsets {
    NSValue *value = objc_getAssociatedObject(self, &KEY_HIT_TEST_EDGE_INSETS);
    if(value) {
        UIEdgeInsets edgeInsets; [value getValue:&edgeInsets]; return edgeInsets;
    }else {
        return UIEdgeInsetsZero;
    }
}

- (BOOL)pointInside:(CGPoint)point withEvent:(UIEvent *)event {
    if(UIEdgeInsetsEqualToEdgeInsets(self.hitTestEdgeInsets, UIEdgeInsetsZero) || !self.enabled || self.hidden) {
        return [super pointInside:point withEvent:event];
    }
    
    CGRect relativeFrame = self.bounds;
    CGRect hitFrame = UIEdgeInsetsInsetRect(relativeFrame, self.hitTestEdgeInsets);
    
    return CGRectContainsPoint(hitFrame, point);
}

@end

```

## UILabel 文本靠左上角

```objc

// .h
@interface BWLeftTopLabel : UILabel
@end

// .m
@implementation BWLeftTopLabel
- (id)initWithFrame:(CGRect)frame {
    return [super initWithFrame:frame];
}

- (CGRect)textRectForBounds:(CGRect)bounds limitedToNumberOfLines:(NSInteger)numberOfLines {
    CGRect textRect = [super textRectForBounds:bounds limitedToNumberOfLines:numberOfLines];
    textRect.origin.y = bounds.origin.y;
    return textRect;    
}

-(void)drawTextInRect:(CGRect)requestedRect {
    CGRect actualRect = [self textRectForBounds:requestedRect limitedToNumberOfLines:self.numberOfLines];
    [super drawTextInRect:actualRect];   
}
@end

```

## UILabel 设置行间隙

```objc
/**
 设置固定行间距文本
 
 @param lineSpace 行间距
 @param text 文本内容
 @param label 要设置的label
 */
-(void)setLineSpace:(CGFloat)lineSpace withText:(NSString *)text inLabel:(UILabel *)label{
    if (!text || !label) {
        return;
    }
    NSMutableParagraphStyle *paragraphStyle = [[NSMutableParagraphStyle alloc] init];
    paragraphStyle.lineSpacing = lineSpace;  //设置行间距
    paragraphStyle.lineBreakMode = label.lineBreakMode;
    paragraphStyle.alignment = label.textAlignment;
    
    NSMutableAttributedString *attributedString = [[NSMutableAttributedString alloc] initWithString:text];
    [attributedString addAttribute:NSParagraphStyleAttributeName value:paragraphStyle range:NSMakeRange(0, [text length])];
    label.attributedText = attributedString;
}

// 使用
  [self setLineSpace:5 withText:row.descStr inLabel:self.descLabel];

```

## 去除 String 中的空格

1. 仅去除前后的空格

```objc
    NSString *str  = [NSString stringWithFormat:@"    sda  sda    "];
    str = [str stringByTrimmingCharactersInSet:[NSCharacterSet whitespaceCharacterSet]];
    NSLog(@"%@", str);  // sda  sda
```

2. 去除所有空格

```objc
    NSString *str = [NSString stringWithFormat:@"   你 好 嘛  ， 跟谁 俩 呢 ！  "];
    str = [str stringByReplacingOccurrencesOfString:@" " withString:@""];
    NSLog(@"%@", str);  // 你好嘛，跟谁俩呢!
```

## UILabel 部分文字可点击

```objc
// .h 


@protocol RichTextDelegate <NSObject>
@optional
/**
 *  RichTextDelegate
 *
 *  @param string  点击的字符串
 *  @param range   点击的字符串range
 *  @param index   点击的字符在数组中的index
 */
- (void)didClickRichText:(NSString *)string
                   range:(NSRange)range
                   index:(NSInteger)index;
@end

@interface UILabel (RichLabel)


/**
 *  是否打开点击效果，默认是打开
 */
@property (nonatomic, assign) BOOL enabledClickEffect;

/**
 *  点击效果颜色 默认lightGrayColor
 */
@property (nonatomic, strong) UIColor *clickEffectColor;

/**
 *  给文本添加Block点击事件回调
 *
 *  @param strings  需要添加的字符串数组
 *  @param clickAction 点击事件回调
 */
- (void)clickRichTextWithStrings:(NSArray <NSString *> *)strings
                     clickAction:(void (^) (NSString *string, NSRange range, NSInteger index))clickAction;

/**
 *  给文本添加点击事件delegate回调
 *
 *  @param strings  需要添加的字符串数组
 *  @param delegate 富文本代理
 */
- (void)clickRichTextWithStrings:(NSArray <NSString *> *)strings
                        delegate:(id <RichTextDelegate> )delegate;

@end
```

```objc
// .m


//
//  UILabel+RichLabel.m
//  BWApp
//
//  Created by wenbo.sun on 2019/9/7.
//  Copyright © 2019 UCAR. All rights reserved.
//

#import "UILabel+RichLabel.h"

#import <objc/runtime.h>
#import <CoreText/CoreText.h>
#import <Foundation/Foundation.h>


#define weakSelf(type)      __weak typeof(type) weak##type = type;

@interface RichTextModel : NSObject

@property (nonatomic, copy) NSString *str;

@property (nonatomic, assign) NSRange range;

@end

@implementation RichTextModel

@end


@implementation UILabel (RichLabel)


#pragma mark - AssociatedObjects

- (NSMutableArray *)attributeStrings {
    
    return objc_getAssociatedObject(self, _cmd);
}

- (void)setAttributeStrings:(NSMutableArray *)attributeStrings {
    
    objc_setAssociatedObject(self, @selector(attributeStrings), attributeStrings, OBJC_ASSOCIATION_RETAIN_NONATOMIC);
}

- (NSMutableDictionary *)effectDic {
    
    return objc_getAssociatedObject(self, _cmd);
}

- (void)setEffectDic:(NSMutableDictionary *)effectDic {
    
    objc_setAssociatedObject(self, @selector(effectDic), effectDic, OBJC_ASSOCIATION_RETAIN_NONATOMIC);
}

- (BOOL)isClickAction {
    
    return [objc_getAssociatedObject(self, _cmd) boolValue];
}

- (void)setIsClickAction:(BOOL)isClickAction {
    
    objc_setAssociatedObject(self, @selector(isClickAction), @(isClickAction), OBJC_ASSOCIATION_ASSIGN);
}

- (void (^)(NSString *, NSRange, NSInteger))clickBlock {
    
    return objc_getAssociatedObject(self, _cmd);
}

- (void)setClickBlock:(void (^)(NSString *, NSRange, NSInteger))clickBlock {
    
    objc_setAssociatedObject(self, @selector(clickBlock), clickBlock, OBJC_ASSOCIATION_COPY_NONATOMIC);
}

- (id<RichTextDelegate>)delegate {
    
    return objc_getAssociatedObject(self, _cmd);
}

- (BOOL)enabledClickEffect {
    
    return [objc_getAssociatedObject(self, _cmd) boolValue];
}

- (void)setEnabledClickEffect:(BOOL)enabledClickEffect {
    
    objc_setAssociatedObject(self, @selector(enabledClickEffect), @(enabledClickEffect), OBJC_ASSOCIATION_ASSIGN);
    //    self.isClickEffect = enabledClickEffect;
}

- (UIColor *)clickEffectColor {
    
    UIColor *obj = objc_getAssociatedObject(self, _cmd);
    if(obj == nil) {obj = [UIColor lightGrayColor];}
    return obj;
}

- (void)setClickEffectColor:(UIColor *)clickEffectColor {
    
    objc_setAssociatedObject(self, @selector(clickEffectColor), clickEffectColor, OBJC_ASSOCIATION_RETAIN_NONATOMIC);
}

- (BOOL)isClickEffect {
    
    return [objc_getAssociatedObject(self, _cmd) boolValue];
}

- (void)setIsClickEffect:(BOOL)isClickEffect {
    
    objc_setAssociatedObject(self, @selector(isClickEffect), @(isClickEffect), OBJC_ASSOCIATION_ASSIGN);
}

- (void)setDelegate:(id<RichTextDelegate>)delegate {
    
    objc_setAssociatedObject(self, @selector(delegate), delegate, OBJC_ASSOCIATION_ASSIGN);
}

#pragma mark - mainFunction
- (void)clickRichTextWithStrings:(NSArray<NSString *> *)strings clickAction:(void (^)(NSString *, NSRange, NSInteger))clickAction {
    
    [self richTextRangesWithStrings:strings];
    
    if (self.clickBlock != clickAction) {
        self.clickBlock = clickAction;
    }
}

- (void)clickRichTextWithStrings:(NSArray<NSString *> *)strings delegate:(id<RichTextDelegate>)delegate {
    
    [self richTextRangesWithStrings:strings];
    
    if ([self delegate] != delegate) {
        
        [self setDelegate:delegate];
    }
}

#pragma mark - touchAction
- (void)touchesBegan:(NSSet<UITouch *> *)touches withEvent:(UIEvent *)event
{
    if (!self.isClickAction) {
        return;
    }
    
    if (objc_getAssociatedObject(self, @selector(enabledClickEffect))) {
        self.isClickEffect = self.enabledClickEffect;
    }
    
    UITouch *touch = [touches anyObject];
    
    CGPoint point = [touch locationInView:self];
    
    weakSelf(self);
    [self richTextFrameWithTouchPoint:point result:^(NSString *string, NSRange range, NSInteger index) {
        
        if (weakself.clickBlock) {
            weakself.clickBlock (string , range , index);
        }
        
        if ([weakself delegate] && [[weakself delegate] respondsToSelector:@selector(didClickRichText:range:index:)]) {
            [[weakself delegate] didClickRichText:string range:range index:index];
        }
        
        if (weakself.isClickEffect) {
            
            [weakself saveEffectDicWithRange:range];
            
            [weakself clickEffectWithStatus:YES];
        }
    }];
}

- (UIView *)hitTest:(CGPoint)point withEvent:(UIEvent *)event {
    
    if((self.isClickAction) && ([self richTextFrameWithTouchPoint:point result:nil])) {
        
        return self;
    }
    return [super hitTest:point withEvent:event];
}

#pragma mark - getClickFrame
- (BOOL)richTextFrameWithTouchPoint:(CGPoint)point result:(void (^) (NSString *string , NSRange range , NSInteger index))resultBlock
{
    CTFramesetterRef framesetter = CTFramesetterCreateWithAttributedString((CFAttributedStringRef)self.attributedText);
    
    CGMutablePathRef Path = CGPathCreateMutable();
    
    CGPathAddRect(Path, NULL, CGRectMake(0, 0, self.bounds.size.width, self.bounds.size.height));
    
    CTFrameRef frame = CTFramesetterCreateFrame(framesetter, CFRangeMake(0, 0), Path, NULL);
    
    CFRange range = CTFrameGetVisibleStringRange(frame);
    
    if (self.attributedText.length > range.length) {
        
        UIFont *font ;
        
        if ([self.attributedText attribute:NSFontAttributeName atIndex:0 effectiveRange:nil]) {
            
            font = [self.attributedText attribute:NSFontAttributeName atIndex:0 effectiveRange:nil];
            
        }else if (self.font){
            font = self.font;
            
        }else {
            font = [UIFont systemFontOfSize:17];
        }
        
        CGPathRelease(Path);
        
        Path = CGPathCreateMutable();
        
        CGPathAddRect(Path, NULL, CGRectMake(0, 0, self.bounds.size.width, self.bounds.size.height + font.lineHeight));
        
        frame = CTFramesetterCreateFrame(framesetter, CFRangeMake(0, 0), Path, NULL);
    }
    
    CFArrayRef lines = CTFrameGetLines(frame);
    
    if (!lines) {
        CFRelease(frame);
        CFRelease(framesetter);
        CGPathRelease(Path);
        return NO;
    }
    
    CFIndex count = CFArrayGetCount(lines);
    
    CGPoint origins[count];
    
    CTFrameGetLineOrigins(frame, CFRangeMake(0, 0), origins);
    
    CGAffineTransform transform = [self transformForCoreText];
    
    CGFloat verticalOffset = 0;
    
    for (CFIndex i = 0; i < count; i++) {
        CGPoint linePoint = origins[i];
        
        CTLineRef line = CFArrayGetValueAtIndex(lines, i);
        
        CGRect flippedRect = [self getLineBounds:line point:linePoint];
        
        CGRect rect = CGRectApplyAffineTransform(flippedRect, transform);
        
        rect = CGRectInset(rect, 0, 0);
        
        rect = CGRectOffset(rect, 0, verticalOffset);
        
        NSParagraphStyle *style = [self.attributedText attribute:NSParagraphStyleAttributeName atIndex:0 effectiveRange:nil];
        
        CGFloat lineSpace;
        
        if (style) {
            lineSpace = style.lineSpacing;
        }else {
            lineSpace = 0;
        }
        
        CGFloat lineOutSpace = (self.bounds.size.height - lineSpace * (count - 1) -rect.size.height * count) / 2;
        
        rect.origin.y = lineOutSpace + rect.size.height * i + lineSpace * i;
        
        if (CGRectContainsPoint(rect, point)) {
            
            CGPoint relativePoint = CGPointMake(point.x - CGRectGetMinX(rect), point.y - CGRectGetMinY(rect));
            
            CFIndex index = CTLineGetStringIndexForPosition(line, relativePoint);
            
            CGFloat offset;
            
            CTLineGetOffsetForStringIndex(line, index, &offset);
            
            if (offset > relativePoint.x) {
                index = index - 1;
            }
            
            NSInteger link_count = self.attributeStrings.count;
            
            for (int j = 0; j < link_count; j++) {
                
                RichTextModel *model = self.attributeStrings[j];
                
                NSRange link_range = model.range;
                if (NSLocationInRange(index, link_range)) {
                    if (resultBlock) {
                        resultBlock (model.str , model.range , (NSInteger)j);
                    }
                    CFRelease(frame);
                    CFRelease(framesetter);
                    CGPathRelease(Path);
                    return YES;
                }
            }
        }
    }
    CFRelease(frame);
    CFRelease(framesetter);
    CGPathRelease(Path);
    return NO;
}

- (void)touchesEnded:(NSSet<UITouch *> *)touches withEvent:(UIEvent *)event
{
    if (self.isClickEffect) {
        
        [self performSelectorOnMainThread:@selector(clickEffectWithStatus:) withObject:nil waitUntilDone:NO];
    }
}

- (void)touchesCancelled:(NSSet<UITouch *> *)touches withEvent:(UIEvent *)event
{
    if (self.isClickEffect) {
        
        [self performSelectorOnMainThread:@selector(clickEffectWithStatus:) withObject:nil waitUntilDone:NO];
    }
}

- (CGAffineTransform)transformForCoreText
{
    return CGAffineTransformScale(CGAffineTransformMakeTranslation(0, self.bounds.size.height), 1.f, -1.f);
}

- (CGRect)getLineBounds:(CTLineRef)line point:(CGPoint)point
{
    CGFloat ascent = 0.0f;
    CGFloat descent = 0.0f;
    CGFloat leading = 0.0f;
    CGFloat width = (CGFloat)CTLineGetTypographicBounds(line, &ascent, &descent, &leading);
    CGFloat height = ascent + fabs(descent) + leading;
    
    return CGRectMake(point.x, point.y , width, height);
}

#pragma mark - clickEffect
- (void)clickEffectWithStatus:(BOOL)status
{
    if (self.isClickEffect) {
        NSMutableAttributedString *attStr = [[NSMutableAttributedString alloc] initWithAttributedString:self.attributedText];
        
        NSMutableAttributedString *subAtt = [[NSMutableAttributedString alloc] initWithAttributedString:[[self.effectDic allValues] firstObject]];
        
        NSRange range = NSRangeFromString([[self.effectDic allKeys] firstObject]);
        
        if (status) {
            [subAtt addAttribute:NSBackgroundColorAttributeName value:self.clickEffectColor range:NSMakeRange(0, subAtt.string.length)];
            
            [attStr replaceCharactersInRange:range withAttributedString:subAtt];
        }else {
            
            [attStr replaceCharactersInRange:range withAttributedString:subAtt];
        }
        self.attributedText = attStr;
    }
}

- (void)saveEffectDicWithRange:(NSRange)range
{
    self.effectDic = [NSMutableDictionary dictionary];
    
    NSAttributedString *subAttribute = [self.attributedText attributedSubstringFromRange:range];
    
    [self.effectDic setObject:subAttribute forKey:NSStringFromRange(range)];
}

#pragma mark - getRange
- (void)richTextRangesWithStrings:(NSArray <NSString *>  *)strings
{
    if (self.attributedText == nil) {
        self.isClickAction = NO;
        return;
    }
    
    self.isClickAction = YES;
    
    self.isClickEffect = YES;
    
    __block  NSString *totalStr = self.attributedText.string;
    
    self.attributeStrings = [NSMutableArray array];
    
    weakSelf(self);
    [strings enumerateObjectsUsingBlock:^(NSString * _Nonnull obj, NSUInteger idx, BOOL * _Nonnull stop) {
        
        NSRange range = [totalStr rangeOfString:obj];
        
        if (range.length != 0) {
            
            totalStr = [totalStr stringByReplacingCharactersInRange:range withString:[weakself getStringWithRange:range]];
            
            RichTextModel *model = [[RichTextModel alloc]init];
            
            model.range = range;
            
            model.str = obj;
            
            [weakself.attributeStrings addObject:model];
        }
    }];
}

- (NSString *)getStringWithRange:(NSRange)range
{
    NSMutableString *string = [NSMutableString string];
    
    for (int i = 0; i < range.length ; i++) {
        
        [string appendString:@" "];
    }
    return string;
}


@end
```

```objc
// 使用


- (void)cellWillAppear {
    [super cellWillAppear];
    
    CKBindVehicleTipCellRow *row = (CKBindVehicleTipCellRow *)self.tableViewRow;
    
    self.tiplabel.text = row.tipStr;
    
    NSString *text = row.tipStr;
    
    NSRange phoneRange = [row.tipStr rangeOfString:row.phoneStr];
    
    NSMutableAttributedString *string = [[NSMutableAttributedString alloc] initWithString:text];

    [string addAttributes:@{NSStrikethroughStyleAttributeName:@"",NSForegroundColorAttributeName:UCAR_ColorFromHexString(@"2D72D9")}  range:phoneRange];
    self.tiplabel.userInteractionEnabled = true;
    self.tiplabel.attributedText = string;

    [self.tiplabel clickRichTextWithStrings:@[row.phoneStr] clickAction:^(NSString *string, NSRange range, NSInteger index) {
        
        NSString *str = [row.phoneStr stringByReplacingOccurrencesOfString:@" " withString:@""];
        NSLog(@"电话 ：%@", str);
        
    }];
}
```

## 找到所有 subviewClass 类
```objc
- (NSMutableArray *)_findSubViews:(UIView *)currentView subViewClass:(NSString *)subviewClass array:(NSMutableArray *)array {
    if (currentView.subviews.count == 0) {
        return array;
    }
    if (!array) {
        array = [NSMutableArray arrayWithCapacity:0];
    } 
    for (NSInteger i = 0; i < currentView.subviews.count; i++) {
        UIView *subb = currentView.subviews[i];
       if ([subb isKindOfClass:NSClassFromString(subviewClass)]) {
           [array addObject:subb];
        }
        
        [self _findSubViews:subb subViewClass:subviewClass array:array];
    }
    return array;
}
```

## 找到 subviewClass 这个类的父视图
```objc

- (UIView *)_findParentView:(UIView *)currentView subViewClass:(NSString *)subviewClass{
    // 深度优先查找
    for (NSInteger i = 0; i < currentView.subviews.count; i++) {
        UIView *subb = currentView.subviews[i];
       if ([subb isKindOfClass:NSClassFromString(subviewClass)]) {
           return currentView;
           break;
        }
        UIView *n = [self _findParentView:subb subViewClass:subviewClass];
        if (n) {
            return n;
            break;
        }
    }
    return nil;
}
```

## iOS13 适配

1. present出来的控制器默认不是全屏

```swift
    let v = WBTestViewController()
    v.modalPresentationStyle = .fullScreen // 加上这句话
    self.present(v, animated: true, completion: nil)
```

2. Dark Mode适配

## RAC 通知的移除

+ [参考链接](https://juejin.im/post/5a30974ef265da433562bec2)
  
```objc
    RACSignal *ss = [[NSNotificationCenter defaultCenter] rac_addObserverForName:@"UserSyncVerifyInfoWithServerSuccessNoti" object:nil];
    
    self.disposableObj = [ss subscribeNext:^(id  _Nullable x) {
        NSLog(@"更新认证信息成功~!!!!!!");
        [vcObjc.view bw_hiddenLoading];

        NSNotification *noti = (NSNotification *)x;
        BOOL syncSuccess = ((NSNumber *)noti.object).boolValue;
        if (syncSuccess) {
            NSLog(@"同步后台成功 - 更新认证信息成功~!!!!!");
        } else {
            NSLog(@"同步后台失败");
        }
        
        [UserRealNameAuthTool _handleToRealNameAuth:params];
        [self.disposableObj dispose];//rac 移除通知监听  
    }];
```

## 类方法里使用 self

```objc
@interface CKTool : NSObject 

+ (void)test0;
+ (void)test1;

@end

@implementation CKTool

+ (void)test0 {
    [self test1]; //效果和👇一样一样
    // [CKTool test1];
}

+ (void)test1 {
    NSLog(@"test 1");
}
@end
```

## 拍照后修复图片方向 `fixOrientation` & 剪切图片 `imageByCroppingWithRect`

```objc
// .h

@interface UIImage (BWCrop)
+ (UIImage *)fixOrientation:(UIImage *)aImage;
- (UIImage *)imageByCroppingWithRect:(CGRect)rect;
@end

// .m 
@implementation UIImage (BWCrop)

+ (UIImage *)fixOrientation:(UIImage *)aImage; {
    if  (aImage.imageOrientation  ==  UIImageOrientationUp)
    return  aImage;
    CGAffineTransform  transform  =  CGAffineTransformIdentity;
    switch  (aImage.imageOrientation)  {
                case  UIImageOrientationDown:
                case  UIImageOrientationDownMirrored:
                        transform  =  CGAffineTransformTranslate(transform,  aImage.size.width,  aImage.size.height);
                        transform  =  CGAffineTransformRotate(transform,  M_PI);
                        break;
                            
                case  UIImageOrientationLeft:
                case  UIImageOrientationLeftMirrored:
                        transform  =  CGAffineTransformTranslate(transform,  aImage.size.width,  0);
                        transform  =  CGAffineTransformRotate(transform,  M_PI_2);
                        break;
                            
                case  UIImageOrientationRight:
                case  UIImageOrientationRightMirrored:
                        transform  =  CGAffineTransformTranslate(transform,  0,  aImage.size.height);
                        transform  =  CGAffineTransformRotate(transform,  -M_PI_2);
                        break;
                default:
                        break;
        }
            
        switch  (aImage.imageOrientation)  {
                case  UIImageOrientationUpMirrored:
                case  UIImageOrientationDownMirrored:
                        transform  =  CGAffineTransformTranslate(transform,  aImage.size.width,  0);
                        transform  =  CGAffineTransformScale(transform,  -1,  1);
                        break;
                            
                case  UIImageOrientationLeftMirrored:
                case  UIImageOrientationRightMirrored:
                        transform  =  CGAffineTransformTranslate(transform,  aImage.size.height,  0);
                        transform  =  CGAffineTransformScale(transform,  -1,  1);
                        break;
                default:
                        break;
        }
            
        //  Now  we  draw  the  underlying  CGImage  into  a  new  context,  applying  the  transform
        //  calculated  above.
        CGContextRef  ctx  =  CGBitmapContextCreate(NULL,  aImage.size.width,  aImage.size.height,
                                                                                          CGImageGetBitsPerComponent(aImage.CGImage),  0,
                                                                                          CGImageGetColorSpace(aImage.CGImage),
                                                                                          CGImageGetBitmapInfo(aImage.CGImage));
        CGContextConcatCTM(ctx,  transform);
        switch  (aImage.imageOrientation)  {
                case  UIImageOrientationLeft:
                case  UIImageOrientationLeftMirrored:
                case  UIImageOrientationRight:
                case  UIImageOrientationRightMirrored:
                        //  Grr...
                        CGContextDrawImage(ctx,  CGRectMake(0,0,aImage.size.height,aImage.size.width),  aImage.CGImage);
                        break;
                            
                default:
                        CGContextDrawImage(ctx,  CGRectMake(0,0,aImage.size.width,aImage.size.height),  aImage.CGImage);
                        break;
        }
            
        //  And  now  we  just  create  a  new  UIImage  from  the  drawing  context
        CGImageRef  cgimg  =  CGBitmapContextCreateImage(ctx);
        UIImage  *img  =  [UIImage  imageWithCGImage:cgimg];
        CGContextRelease(ctx);
        CGImageRelease(cgimg);
        return  img;
}

- (UIImage *)imageByCroppingWithRect:(CGRect)rect { 
    CGImageRef imageRef = self.CGImage;
    CGImageRef imagePartRef = CGImageCreateWithImageInRect(imageRef, rect);
    UIImage *cropImage = [UIImage imageWithCGImage:imagePartRef];
    CGImageRelease(imagePartRef); 
    return cropImage;
}
@end

```
## 设置APP支持的文件类型 eg:PDF

+ [Core Foundation Keys](https://developer.apple.com/library/archive/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/uid/20001431-101685)
+ [System-Declared Uniform Type Identifiers
](https://developer.apple.com/library/archive/documentation/Miscellaneous/Reference/UTIRef/Articles/System-DeclaredUniformTypeIdentifiers.html)

// todo

## `Bundle.main.paths(forResourcesOfType: "pdf", inDirectory: "swift_lang")` 方法获取不到文件解决

导入文件的时候选取create folder references

![](../../src/imgs/ios/create_folder_references.png)

![](../../src/imgs/ios/create_folder_references_result.png)

![](../../src/imgs/ios/create_folder_references_code.png)

## Xcode11 新建项目，去除 SceneDelegate.swift

 - 删除 SceneDelegate.swift 文件
 - info.plist 中移除 `Application Scene Manifest` 项
    ![](../../src/imgs/ios/swift_tip/secen_plist.png)
 - 注释掉相关代码
   ```swift
   func application(_ application: UIApplication, configurationForConnecting connectingSceneSession: UISceneSession, options: UIScene.ConnectionOptions) -> UISceneConfiguration { 
   }

   func application(_ application: UIApplication, didDiscardSceneSessions sceneSessions: Set<UISceneSession>) { 
   }
   ```
 - 新增window属性
   ```swift
   var win: UIWindow?

   func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool { 
       win = UIWindow.init(frame: UIScreen.main.bounds)
        win?.rootViewController = UIStoryboard.init(name: "Main", bundle: nil).instantiateInitialViewController()
        win?.makeKeyAndVisible()
       return true
     } 
   ```
## Xcode 报错
**编译报错：xxx.modulemap' has been modified since the precompiled header 'xxx.pch.pch' was built**

解决：clean下工程


## 旋转动画
```objc
CABasicAnimation *animation = [CABasicAnimation animationWithKeyPath:@"transform.rotation.z"];
  // 默认是顺时针效果，若将fromValue和toValue的值互换，则为逆时针效果
  animation.fromValue = [NSNumber numberWithFloat:0.f];
  animation.toValue = [NSNumber numberWithFloat: M_PI *2];
  animation.duration = 1;
  animation.autoreverses = NO;
  animation.fillMode = kCAFillModeForwards;
  // 如果这里想设置成一直自旋转，可以设置为MAXFLOAT，否则设置具体的数值则代表执行多少次
  animation.repeatCount = MAXFLOAT;
  [self.indicatorView.layer addAnimation:animation forKey:nil];


  // [self.indicatorView.layer removeAllAnimations];
```

## 方法废弃

```objc
- (instancetype)initWithVin:(NSString *)vin;
- (instancetype)init DEPRECATED_MSG_ATTRIBUTE("使用 initWithVin");
```

## NSURL 的 query 、path 等方法
```objc
NSURL *url = [NSURL URLWithString:@"http://www.testurl.com:8080/subpath/subsubpath?uid=123&gid=456"];  
[url scheme]  // http  
[url host]  // www.testurl.com  
[url port]  // 8080  
[url path]  // /subpath/subsubpath  
[url lastPathComponent]  // subsubpath  
[url query]     // uid=123&gid=456  
```

## 修改 UIPickerView 中的文字大小
```objc
- (UIView *)pickerView:(UIPickerView *)pickerView viewForRow:(NSInteger)row forComponent:(NSInteger)component reusingView:(UIView *)view { 
    NSString *titleString = self.typeArray[row]; 
    
    UILabel *itemlabel = [[UILabel alloc] init];
    itemlabel.attributedText = [[NSAttributedString alloc] initWithString:titleString
                                                               attributes:@{
                                                                   NSFontAttributeName: [UIFont systemFontOfSize:16],
                                                                   NSForegroundColorAttributeName: UCAR_ColorFromHexStringAndAlpha(@"#333333", (1))}];
        
    return itemlabel;
}
```
 

## 深拷贝
```objc
// .h
@interface NSObject (UCARDeepCopy)
- (void)deepCopy:(NSObject *)originObj;
@end

// .m
#import <objc/runtime.h>
@implementation NSObject (UCARDeepCopy)

- (void)deepCopy:(NSObject *)originObj {
    unsigned int property_count = 0;
    objc_property_t * propertys = class_copyPropertyList([originObj class], &property_count);
    for (int i = 0; i < property_count; i++) {
        objc_property_t property = propertys[i];
        const char * property_name = property_getName(property);
        NSString * property_name_string = [NSString stringWithUTF8String:property_name];
        [self setValue:[originObj valueForKey:property_name_string] forKey:property_name_string];
    }
    free(propertys);
}
@end
```

## [Application] The app delegate must implement the window property if it wants to use a main storyboard file.

终端log出上面一段话，解决方式是添加 window 属性

![](./../../src/imgs/ios/xcode_error_implement.png)
```swift
var window: UIWindow?

func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool { 
    window = UIWindow.init(frame: UIScreen.main.bounds)
    window?.rootViewController = UIStoryboard.init(name: "Main", bundle: nil).instantiateInitialViewController()
    window?.makeKeyAndVisible() 
    return true
}
```
## 秒数转成 00:00:00 格式  eg: 60s -> 00:01:00
```objc 
+ (NSString *)timeStringWithDuration:(NSTimeInterval)duration {
    NSInteger seconds ;
    NSInteger mins ;
    NSInteger hours ;
    
    if (duration < 60) {
        seconds = duration;
        mins = 0;
        hours = 0;
    } else if (duration >= 60 && duration < 3600) {
        seconds = (int)duration % 60;
        mins = duration / 60;
        hours = 0;
    } else {
        hours = (int)duration / 3600;
        mins = ((int)duration % 3600) / 60;
        seconds = ((int)duration % 3600) % 60;
    }
    
    NSString *hourString = hours < 10 ? [NSString stringWithFormat:@"0%ld", (long)hours] : [NSString stringWithFormat:@"%ld", (long)hours];
    NSString *minString = mins < 10 ? [NSString stringWithFormat:@"0%ld", (long)mins] : [NSString stringWithFormat:@"%ld", (long)mins];
    NSString *secondString = seconds < 10 ? [NSString stringWithFormat:@"0%ld", (long)seconds] : [NSString stringWithFormat:@"%ld",(long)seconds];
    NSString *result = [NSString stringWithFormat:@"%@:%@:%@", hourString, minString, secondString];
    
    return result;
}s
```

## 添加 pch 文件时候路径怎么写
![](./../../src/imgs/ios/pch_path.png)

## iOS 添加点击效果，方便录屏时候看触点
```objc
//
//  UIWindow+UCARRobot.m
//  UCARRobot
//
//  Created by wb on 2020/4/3.
//

#import "UIWindow+UCARRobot.h" 
#import <objc/runtime.h>

@implementation UIWindow (UCARRobot)

+ (void)load {
    Method m1 = class_getInstanceMethod([self class], @selector(sendEvent:));
    Method m2 = class_getInstanceMethod([self class], @selector(ucar_sendEvent:));
    method_exchangeImplementations(m1, m2);
}

- (void)ucar_sendEvent:(UIEvent *)event {
    [self ucar_sendEvent:event];
    [self dealTouch:event];
}

- (void)dealTouch:(UIEvent *)event {
    UITouch *touch = event.allTouches.anyObject;
    if (touch.phase == UITouchPhaseEnded) {
        return;
    }
    
   NSNumber *value = [[NSUserDefaults standardUserDefaults] valueForKey:@"UCARTouchAnimationOn_Key"];
    if (!value.boolValue) {
        return;
    }
    
    static CGFloat width = 20;
    if (event.type == UIEventTypeTouches) {
        
        CGPoint point = [event.allTouches.anyObject locationInView:self];
        
        CGFloat oringX = point.x - width / 2;
        CGFloat oringY = point.y - width / 2;
        CGRect rect = CGRectMake(oringX, oringY, width, width);
        UIView *blackV = [[UIView alloc] initWithFrame:rect];
        blackV.alpha = 0.3;
        blackV.layer.cornerRadius = width / 2;
        blackV.backgroundColor = [UIColor purpleColor];
        [self addSubview:blackV];
        [self bringSubviewToFront:blackV];
        // 设置动画
        CABasicAnimation *animation = [CABasicAnimation animationWithKeyPath:@"transform.scale"];
        animation.duration = 0.3;
        animation.fromValue = @1;
        animation.toValue = @2;
        animation.fillMode = @"backwards";
        animation.removedOnCompletion = YES;
        [blackV.layer addAnimation:animation forKey:@"an1"];
        
        dispatch_after(dispatch_time(DISPATCH_TIME_NOW, (int64_t)(0.27 * NSEC_PER_SEC)), dispatch_get_main_queue(), ^{
            [blackV removeFromSuperview];
        });
    }
}

@end

```

## model类转字典
```objc

+ (NSDictionary*)getObjectData:(id)obj{
    NSMutableDictionary *dic = [NSMutableDictionary dictionary];
    unsigned int propsCount;
    objc_property_t *props = class_copyPropertyList([obj class], &propsCount);//获得属性列表
    for(int i = 0;i < propsCount; i++){
        objc_property_t prop = props[i];
        NSString *propName = [NSString stringWithUTF8String:property_getName(prop)];//获得属性的名称
        id value = [obj valueForKey:propName];//kvc读值
        if(value == nil){
            value = [NSNull null];
        }else{
            value = [self getObjectInternal:value];//自定义处理数组，字典，其他类
        }
        [dic setObject:value forKey:propName];
    }
    return dic;
}

+ (id)getObjectInternal:(id)obj{
    if([obj isKindOfClass:[NSString class]] || [obj isKindOfClass:[NSNumber class]] || [obj isKindOfClass:[NSNull class]]) {
        return obj;
    }
    if([obj isKindOfClass:[NSArray class]]) {
        NSArray *objarr = obj;
        NSMutableArray *arr = [NSMutableArray arrayWithCapacity:objarr.count];
        for(int i = 0;i < objarr.count; i++) {
            [arr setObject:[self getObjectInternal:[objarr objectAtIndex:i]] atIndexedSubscript:i];
        }
        return arr;
    }
    if([obj isKindOfClass:[NSDictionary class]]) {
        NSDictionary *objdic = obj;
        NSMutableDictionary *dic = [NSMutableDictionary dictionaryWithCapacity:[objdic count]];
        for(NSString *key in objdic.allKeys){
            [dic setObject:[self getObjectInternal:[objdic objectForKey:key]] forKey:key];
        }
        return dic;
    }
    return [self getObjectData:obj];
}
```

## iOS10上的 navgaitionBarItem 不显示问题

  要设置一个frame，否则10上显示不出来
  
```objc
    UIButton *historyBtn = [UIButton buttonWithType:(UIButtonTypeCustom)];
    historyBtn.frame = CGRectMake(0, 0, 24, 24); //  要设置一个frame，否则10上显示不出来
    [historyBtn setImage:[CKContext imageNamed:@"ck_charge_history"] forState:(UIControlStateNormal)];
    self.navigationItem.rightBarButtonItem = [[UIBarButtonItem alloc] initWithCustomView:historyBtn];
    [historyBtn addTarget:self action:@selector(toHistory) forControlEvents:(UIControlEventTouchUpInside)];
```

## class_copyPropertyList 不能复制父类的属性

- https://www.jianshu.com/p/bfe42b9cb37f

todo

## git 报错：refusing to merge unrelated histories

```shell
git pull origin master --allow-unrelated-histories
```

## 字符串某些变色
```objc
 NSAttributedString *attr0 = [[NSAttributedString alloc] initWithString:[NSString stringWithFormat:@"%d",textView.text.length] attributes:@{
            NSForegroundColorAttributeName: UCAR_ColorFromHexString(@"#F12E49"),
            NSFontAttributeName: [UIFont systemFontOfSize:14]
        }];
        NSAttributedString *attr1 = [[NSAttributedString alloc] initWithString:[NSString stringWithFormat:@"/%d",row.charactersLimit] attributes:@{
            NSForegroundColorAttributeName: UCAR_ColorFromHexString(@"#CCCCCC"),
            NSFontAttributeName: [UIFont systemFontOfSize:14]
        }];
        NSMutableAttributedString *att = [[NSMutableAttributedString alloc] init];
        [att appendAttributedString:attr0];
        [att appendAttributedString:attr1];
        self.countlabel.attributedText = att;
```

## 编译不过，storyboard 报错 : internal error.

![internal](../../src/imgs/ios/internalerror.png)

1. 试着把最近拖进来的视图删掉，配合 cmd + z
2. 试着把视图的宽度约束由<按比例 >改成<固定值>

## UITableView haader 悬浮效果

- plain 样式 header 悬浮
- group 样式取消 section 之间间隔：设置 footer 高度 0.01
```swift
override func tableView(_ tableView: UITableView, heightForFooterInSection section: Int) -> CGFloat {
    return 0.01     
}
```
## 让 UITableViewController 的 tableview 内容在状态栏下
```objc
// 如果iOS的系统是11.0，会有这样一个宏定义“#define __IPHONE_11_0  110000”；如果系统版本低于11.0则没有这个宏定义
  #ifdef __IPHONE_11_0
  if ([self.tableView respondsToSelector:@selector(setContentInsetAdjustmentBehavior:)]) {
      self.tableView.contentInsetAdjustmentBehavior = UIScrollViewContentInsetAdjustmentNever;
  }
  #endif
```
![](../../src/imgs/ios/tableviewcontroller.png)

## 关闭 iOS13 的黑暗模式
info.plist 添加 UIUserInterfaceStyle = Light
![](../../src/imgs/ios/darkoff.png)

## 贝塞尔曲线添加阴影 
```objc
UIView *bgV = [[UIView alloc] initWithFrame:CGRectMake(8 * SCALE, 11 * SCALE, 80 * SCALE, 67 * SCALE)];
bgV.backgroundColor = [UIColor clearColor];
bgV.layer.shadowOffset = CGSizeMake(0, 0);
bgV.layer.shadowColor = UIColorFromRGB(0xD0D0D0).CGColor;
bgV.layer.shadowOpacity = 0.5;
bgV.layer.shadowRadius = 2;
UIBezierPath *path = [UIBezierPath bezierPathWithRect:CGRectMake(-2 * SCALE, -2 * SCALE, 80 * SCALE + 4 * SCALE, 67 * SCALE + 4 * SCALE)];
bgV.layer.shadowPath = path.CGPath;
[self.view addSubview:bgV];
[self.view addSubview:self.topView];
```
## 两个角切圆角
```objc
CGFloat leftMargin = 10.f;
CGFloat hGap = 12.5;
CGFloat cardW = (kScreenWidth - leftMargin * 2 - hGap * 2) / 3;

UIBezierPath *maskPath = [UIBezierPath bezierPathWithRoundedRect:CGRectMake(0, 0, cardW, 17) byRoundingCorners:UIRectCornerTopRight | UIRectCornerTopLeft cornerRadii:CGSizeMake(10, 10)];
CAShapeLayer *maskLayer = [[CAShapeLayer alloc] init];
maskLayer.frame = self.popularlabel.bounds;
maskLayer.path = maskPath.CGPath;
self.popularlabel.layer.mask = maskLayer;
```
## 修改UIAlertAction文字颜色
```objc 
UIAlertAction *action2 = [UIAlertAction actionWithTitle:@"取消" style:UIAlertActionStyleCancel handler:^(UIAlertAction * _Nonnull action) {
    
}]; 
[action2 setValue:[UIColor redColor] forKey:@"titleTextColor"];
```
## 设置 UITextField 和 UIDatePicker 联动
```objc 
- (void)awakeFromNib {
    [super awakeFromNib];
    // Initialization code 

    //创建时间选择对象
    UIDatePicker *datePicker = [[UIDatePicker alloc] init];
    //设置地区: zh-中国
    datePicker.locale = [NSLocale localeWithLocaleIdentifier:@"zh"];
    //设置日期模式 4种
    //    UIDatePickerModeTime,
    //    UIDatePickerModeDate,
    //    UIDatePickerModeDateAndTime,
    //    UIDatePickerModeCountDownTimer,
    datePicker.datePickerMode = UIDatePickerModeDate;
    // 设置当前显示时间
    [datePicker setDate:[NSDate date] animated:YES];
    // 设置显示最大时间（此处为当前时间）
    [datePicker setMaximumDate:[NSDate date]];
    //设置时间格式
    NSDateFormatter *formatter = [[NSDateFormatter alloc] init]; 
    [formatter setDateFormat:@"yyyy-MM-dd"];
    NSString *dateOneString = @"1990-05-02";
    NSDate *dateOne = [formatter dateFromString:dateOneString]; 
    [datePicker setMinimumDate:dateOne]; 
    // 监听DataPicker的滚动 
    [datePicker addTarget:self action:@selector(dateChange:) forControlEvents:UIControlEventValueChanged]; 
    // 设置时间输入框的键盘框样式为时间选择器
    self.birthTextField.inputView = datePicker;
}
- (void)dateChange:(UIDatePicker *)picker {
    NSDateFormatter *formatter = [[NSDateFormatter alloc] init];
    formatter.dateFormat = @"YYYY-MM-dd";
    NSString *str = [formatter stringFromDate:picker.date];
    self.birthTextField.text = str;
}
```
## 使用 CoreLocation 定位
> info.plist 加权限请求 
> Privacy - Location Always Usage Description
> Privacy - Location When In Use Usage Description
```objc
// .h 
@interface CMLocationTool : NSObject 
@property (nonatomic, strong) NSString *latitude;//纬
@property (nonatomic, strong) NSString *longitude;//经 
+ (instancetype)sharedInstance; 
- (void)startUpdateLocation;
- (void)endUpdateLocation; 
@end

// .m

#import "CMLocationTool.h"
#import <CoreLocation/CoreLocation.h>

@interface CMLocationTool () <CLLocationManagerDelegate> {
    CLLocationManager *_locationManager;//定位服务管理类
    CLGeocoder * _geocoder;//初始化地理编码器
}
@end
@implementation CMLocationTool

+ (instancetype)sharedInstance {
    static CMLocationTool *obj = nil;
    static dispatch_once_t onceToken;
    dispatch_once(&onceToken, ^{
        obj = [[CMLocationTool alloc] init];
        [obj initializeLocationService];
    });
    return obj;
}

- (void)initializeLocationService {
    // 初始化定位管理器
    _locationManager = [[CLLocationManager alloc] init];
    [_locationManager requestWhenInUseAuthorization];
    //[_locationManager requestAlwaysAuthorization];//iOS8必须，这两行必须有一行执行，否则无法获取位置信息，和定位
    // 设置代理
    _locationManager.delegate = self;
    // 设置定位精确度到米
    _locationManager.desiredAccuracy = kCLLocationAccuracyBest;
    // 设置过滤器为无
    _locationManager.distanceFilter = kCLDistanceFilterNone;
    //初始化地理编码器
    _geocoder = [[CLGeocoder alloc] init];
}
- (void)startUpdateLocation {
    [_locationManager startUpdatingLocation];// 开始定位之后会不断的执行代理方法更新位置会比较费电所以建议获取完位置即时关闭更新位置服务
}
- (void)endUpdateLocation {
    [_locationManager stopUpdatingLocation]; //不用的时候关闭更新位置服务
}
#pragma mark - CLLocationManagerDelegate
- (void)locationManager:(CLLocationManager *)manager didUpdateLocations:(NSArray<CLLocation *> *)locations {

        NSLog(@"%lu",(unsigned long)locations.count);
        CLLocation * location = locations.lastObject;
        // 纬度
        CLLocationDegrees latitude = location.coordinate.latitude;
        // 经度
        CLLocationDegrees longitude = location.coordinate.longitude;
    
    
    self.latitude = [NSString stringWithFormat:@"%lf", latitude];
    self.longitude = [NSString stringWithFormat:@"%lf", longitude];
    
        NSLog(@"%@",[NSString stringWithFormat:@"%lf", location.coordinate.longitude]);
    //    NSLog(@"经度：%f,纬度：%f,海拔：%f,航向：%f,行走速度：%f", location.coordinate.longitude, location.coordinate.latitude,location.altitude,location.course,location.speed);
        
//        [_geocoder reverseGeocodeLocation:location completionHandler:^(NSArray<CLPlacemark *> * _Nullable placemarks, NSError * _Nullable error) {
//            if (placemarks.count > 0) {
//                CLPlacemark *placemark = [placemarks objectAtIndex:0];
//                NSLog(@"%@",placemark.name);
//                //获取城市
//                NSString *city = placemark.locality;
//                if (!city) {
//                    //四大直辖市的城市信息无法通过locality获得，只能通过获取省份的方法来获得（如果city为空，则可知为直辖市）
//                    city = placemark.administrativeArea;
//                }
//                // 位置名
//        　　NSLog(@"name,%@",placemark.name);
//        　　// 街道
//        　　NSLog(@"thoroughfare,%@",placemark.thoroughfare);
//        　　// 子街道
//        　　NSLog(@"subThoroughfare,%@",placemark.subThoroughfare);
//        　　// 市
//        　　NSLog(@"locality,%@",placemark.locality);
//        　　// 区
//        　　NSLog(@"subLocality,%@",placemark.subLocality);
//        　　// 国家
//        　　NSLog(@"country,%@",placemark.country);
//            }else if (error == nil && [placemarks count] == 0) {
//                NSLog(@"No results were returned.");
//            } else if (error != nil){
//                NSLog(@"An error occurred = %@", error);
//            }
//        }];
}

```
# xib & storyboard

## xib 创建 UIView 
```swift
let v = Bundle.main.loadNibNamed("ExpressSingleInfoView", owner: nil, options: nil)?.last as! ExpressSingleInfoView
```

![](../../src/imgs/ios/xib_uiview.png)

## 获取故事版上的vc
```swift
private class func getVCFromStoryboard(storyboard: String, vcIdentifier: String )-> UIViewController {
        let vc = UIStoryboard.init(name: storyboard, bundle: nil).instantiateViewController(withIdentifier: vcIdentifier)
        return vc;
}
```
## UITableViewController 静态 cell 和动态 cell 混用

> 静态 cell 只能在 UITableViewController 中使用
- 动态section必须要保留1个cell
- cell的缩进级别代理方法，动态静态cell必须重写，否则会造成崩溃
```objc
- (NSInteger)tableView:(UITableView *)tableView numberOfRowsInSection:(NSInteger)section{
    if(section == SectionTypeSKU){// （动态cell）
        return self.pinModel.skuList.count;
    }
    if (section == SectionTypeLimit && !self.switchBtn.on) {
        return 0;
    }
    return [super tableView:tableView numberOfRowsInSection:section];
}

- (UITableViewCell *)tableView:(UITableView *)tableView cellForRowAtIndexPath:(NSIndexPath *)indexPath{
    if(SectionTypeSKU == indexPath.section){//（动态cell）
        SkuInputCell *cell = [SkuInputCell cellWithTableView:tableView];
        return cell;
    }
    return [super tableView:tableView cellForRowAtIndexPath:indexPath];
}

// MARK: - tableviewDelegate

- (CGFloat)tableView:(UITableView *)tableView heightForRowAtIndexPath:(NSIndexPath *)indexPath{
    if(SectionTypeSKU == indexPath.section){//（动态cell）
        return 154;
    }
    return [super tableView:tableView heightForRowAtIndexPath:indexPath];
}

//cell的缩进级别，动态静态cell必须重写，否则会造成崩溃
- (NSInteger)tableView:(UITableView *)tableView indentationLevelForRowAtIndexPath:(NSIndexPath *)indexPath{
    if(SectionTypeSKU == indexPath.section){// （动态cell）
        return [super tableView:tableView indentationLevelForRowAtIndexPath: [NSIndexPath indexPathForRow:0 inSection:indexPath.section]];
    }
    return [super tableView:tableView indentationLevelForRowAtIndexPath:indexPath];
}
```
## 让自定义 view 在 xib 或 storyboard 上也能用

```swift 
/* 创建一个 CustomButtonView    https://www.jianshu.com/p/4c9f9286f293
关键步骤： 
    1. IBDesignable
    2. override func prepareForInterfaceBuilder()
*/
import UIKit

@IBDesignable
class CustomButtonView: UIView {
    
    lazy var label: UILabel = {
        let l = UILabel()
        l.textAlignment = .center
        self.addSubview(l)
        l.snp.makeConstraints { (make) in
            make.left.equalTo(icon.snp.right).offset(5)
            make.centerY.top.equalToSuperview()
            make.right.equalTo(-10)
        }
        return l
    }()
    
    lazy var icon : UIImageView = {
        let img = UIImageView()
        self.addSubview(img)
        img.snp.makeConstraints { (make) in
            make.left.equalTo(10)
            make.centerY.equalToSuperview()
            make.width.equalTo(10)
            make.height.equalTo(14)
        }
        return img
    }()
     
    var tapBlock: DoctorVoidBlock?
    
    lazy var tapBtn: UIButton = {
        let b = UIButton()
        b.addTarget(self, action: #selector(tapAction), for: .touchUpInside)
        self.addSubview(b)
        b.snp.makeConstraints { (make) in
            make.left.top.centerX.centerY.equalToSuperview()
        }
        return b
    }()
    
    @IBInspectable var bgColor: UIColor = UIColor.cyan {
        didSet {
            self.backgroundColor = bgColor
        }
    }
    
    @IBInspectable var iconImg: UIImage? {
        didSet {
            self.icon.image = iconImg
        }
    }
    
    @IBInspectable var labelStr: String? {
        didSet {
            self.label.text = labelStr
        }
    }
    
    @IBInspectable var labelTextFontSize: CGFloat = 12 {
        didSet {
            self.label.font = UIFont.systemFont(ofSize: labelTextFontSize)
        }
    }
    
    @IBInspectable var labelTextColor: UIColor = .white {
           didSet {
               self.label.textColor = labelTextColor
           }
    }
    
    override func prepareForInterfaceBuilder() {
        
    }
    
    @objc func tapAction () {
        if let b = tapBlock {
            b()
        }
    }
}
```
![](../../src/imgs/ios/xib_view.png)