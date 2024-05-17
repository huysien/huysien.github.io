---
layout: post
title: "Tại sao lại chọn Flutter?"
date: 2024-05-17 23:00:00 +0700
categories: tech
author: Huy
comments: true
description: "Trong bài viết này, chúng ta sẽ cùng tìm hiểu tại sao Flutter lại là lựa chọn số 1 khi phát triển ứng dụng đa nền tảng"

---
Đối với một mobile dev, đây có lẽ là một câu hỏi mà bạn sẽ phải đối mặt vào một ngày nào đó. Hôm nay thì mình cũng vừa phải trả lời cho đối tác xong, nên mình cũng chia sẻ lại vào đây một chút vì có thể sẽ cần reuse sau này.

## Câu chuyện đa nền tảng

Trước hết, Flutter là một cross-platform framework, người ta chọn nó vì người ta cần một single codebase cho nhiều nền tảng, giúp tăng tính đồng nhất về mặt logic và giảm chi phí maintain sau này.

Và để nói về những lựa chọn cho cross-platform framework, ở thời điểm hiện tại, chúng ta chỉ còn lại 2 ông lớn là Flutter và React Native để có thể tin tưởng. Những lựa chọn khác như Xamarin, Ionic,... chỉ phục vụ một số nhu cầu nhất định và không phù hợp với phần lớn các ứng dụng thông thường.

## Tại sao lại chọn Flutter thay vì React Native?

- **Performance**: Có thể nói đây là điểm khác biệt và là điểm mạnh lớn nhất của Flutter so với React Native. Flutter compile thành native code cho từng nền tảng, do đó performance (tốc độ rendering, tốc độ xử lý thuật toán,...) tốt hơn hẳn so với việc sử dụng JavaScript bridge như React Native.

- **UI đồng nhất**: Flutter có rendering engine riêng và cung cấp bộ widget rất đồ sộ. Điểm mấu chốt khi có rendering engine riêng đó là app sẽ có được UI và behaviour hoàn toàn đồng nhất trên tất cả các nền tảng.

- **Cộng đồng mạnh và có ông lớn Google đứng phía sau**: Có nghĩa là chúng ta có thể tìm thấy nhiều tài nguyên, thư viện và công cụ hữu ích. Việc tích hợp các dịch vụ của Google cũng rất dễ dàng và rủi ro đem con bỏ chợ cũng giảm đi nhiều.

## Điểm cần cân nhắc khi chọn Flutter

- **Flutter sinh sau đẻ muộn**, do đó số lượng thư viện bên thứ ba có thể sẽ ít hơn và kiến thức từ cộng đồng có thể cũng chưa nhiều bằng. Hiện tại đã là 2024, qua nhiều năm phát triển, cộng đồng Flutter đã trở nên vô cùng lớn mạnh, hầu hết các yêu cầu kỹ thuật đều có thể giải quyết. Tuy nhiên nếu chưa có thư viện hỗ trợ thì cũng cần tăng thêm effort để bridge từ native. Do đó đối với những dự án rất đặc thù, chúng ta nên research trước khả năng đáp ứng các yêu cầu kỹ thuật để estimate cho chuẩn chỉnh.

- **Kích thước app**: Một số nguồn tham khảo cho thấy, Flutter app có thể sẽ có dung lượng lớn hơn khi so sánh với native app hoặc app được build từ platform khác. Do đó, cần xem xét về nhu cầu có khắt khe hay không về mặt dung lượng app mà thiết bị các bạn hỗ trợ có thể có. Nhưng thường thì vấn đề này cũng ít được quan tâm trừ những sản phẩm quá đặc thù.

- **Khả năng tiếp cận**: Flutter sử dụng ngôn ngữ lập trình riêng là Dart, và do đó để tiếp cận Flutter thì chúng ta cần có đội ngũ Flutter dev riêng. Không như JavaScript, một ngôn ngữ cực kì phổ biến đối với thế giới web, có thể bạn chỉ cần kéo vài ông FrontEnd dev sang code là được. Tuy nhiên một thực tế xung quanh mình cho thấy, native mobile dev tiếp cận Dart dễ hơn là JavaScript, mà nếu bạn focus vào Flutter cho mobile, thì nên sử dụng mobile dev. Do đó, để mà nói nên lựa chọn Flutter hay không, phải xem xét đội ngũ của bạn là ai nữa.
