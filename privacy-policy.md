# BaroGuard — Privacy Policy / Chính sách quyền riêng tư

## English

**Effective date:** 2026-10-13
**Contact:** ngothaibao3012@gmail.com

BaroGuard shows the air pressure where you are and lets you note how you feel, so you can look at the two
side by side. This page explains what the app does with your information.

### 1. In short

- Your symptom notes stay on your iPhone. BaroGuard has no account and no server of its own, and it does
  not sync your notes to the cloud.
- To show the air pressure, the app sends an **approximate** location to Apple Weather.
- If you search for a city, what you type goes to Apple Maps.
- The app counts a few anonymous events (such as "the app was opened") through a service called
  TelemetryDeck, together with basic device information and how often and how long the app is used. You can turn this off at any time. It never
  includes your symptoms, your pressure history or your location.
- You can export everything, or delete everything, from Settings.
- BaroGuard is not a medical device (see section 10).

### 2. What the app stores on your device

| What                   | Details                                                                                                                                |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Symptom logs           | The time, how you felt (fine / mild / pain / lying down), and, if you add them, a pain score from 1 to 10 and the medication you took. |
| Pressure history       | Hourly air-pressure readings the app has fetched, and readings from your phone's barometer where it has one.                           |
| Settings and app state | Your pressure unit, your chosen city, whether you finished the introduction, the analytics switch, and a few "already done" markers.   |
| Weather attribution    | The Apple Weather logo and legal link, which Apple requires the app to show.                                                           |

This information is stored only on your device. If you back up your iPhone (to iCloud or to a computer),
the app's data is part of that backup, because that is how iOS backups work. You control backups in iOS
Settings and in Finder. BaroGuard does not upload your data to any server and does not sync it between
devices.

### 3. Location → Apple Weather

If you allow location access (while using the app), the app rounds your position to **0.1 degree, about
10 km**, and sends that rounded position to **Apple Weather (WeatherKit)** to get the current and
forecast pressure. The exact position is not sent. If you prefer, you can choose a city instead of
allowing location. Apple's handling of this request is described in Apple's own privacy documentation.
The app does not send your location to the developer or to the analytics service.

### 4. City search → Apple Maps

When you type in the city search, the text you type is sent to **Apple Maps** (`MKLocalSearchCompleter`) to
suggest places. When you tap one suggestion, the app asks Apple Maps (`MKLocalSearch`) for that one
place's position. The text is not sent anywhere else. The app tells you this on the search screen.

### 5. Phone barometer

On iPhones that have a barometer, the app reads it (with your permission for "Motion & Fitness") to show
the pressure at your phone. This reading stays on the device.

### 6. Anonymous usage statistics (TelemetryDeck)

The app uses **TelemetryDeck**, a privacy-focused analytics service, to learn which parts of the app are
used. This is **on by default**. The first count can be sent while you are going through the
introduction. You can turn it off in **Settings ▸ Your data ▸ Share anonymous usage data**; after that
nothing is sent. Turning it off stops sending from then on; it does not remove counts that were already
received.

**The only events the app can send** (each one is just its name, with no extra information):

| Event                    | Sent when                                                                                                         |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| `opened_app`             | The app comes to the foreground, at most once every 30 minutes                                                    |
| `completed_onboarding`   | You finish the introduction                                                                                       |
| `first_log`              | You save your very first symptom log                                                                              |
| `viewed_forecast`        | You open a day in the 7-day strip, or the strip stays on screen for a moment (once per launch)                    |
| `viewed_history`         | You open the History tab (once per launch)                                                                        |
| `viewed_pattern`         | Defined in the app but **not sent** in this version                                                               |
| `started_trial`          | Only if the subscription screen is switched on in a future version: you start a free trial (once)                 |
| `converted_subscription` | Only if the subscription screen is switched on in a future version: a trial turns into a paid subscription (once) |

**What the TelemetryDeck software adds on its own** to every count. This list was read from the
software's source code (version 2.14.2), so it is what your device sends:

- _App and device:_ app version and build number; iOS version; device model, processor architecture and
  platform; screen size, scale and orientation; whether the app is a TestFlight, App Store, debug or
  simulator build; the name and version of the TelemetryDeck software.
- _Language and settings:_ language, region and locale; time zone; light or dark appearance; layout
  direction (left-to-right or right-to-left); text size; and these accessibility switches: reduce motion,
  bold text, invert colors, darker system colors, reduce transparency, differentiate without color.
- _Date and time:_ day of the month, day of the week, day of the year, week of the year, month, quarter,
  whether it is a weekend, and the hour of the day.
- _Usage-history fields:_ date of the first session, number of days the app was used (in total and in the
  last 30 days), total number of sessions, and the average and previous session length in seconds. The
  software always includes these fields. BaroGuard switches the software's "session statistics" setting
  off, but the software still keeps a list of the days on which the app was used and a running timer of the
  time the app is open, in its own storage on your device, so these numbers can be real. (The "first session
  date" is not recorded in this setup and is simply the date of that count.) They are numbers about how
  often and how long the app is used; they say nothing about you or your health.

**An anonymous identifier.** To count people once, the software uses the iOS "identifier for vendor"
(the same for all apps from this developer on your device, and not your advertising identifier). It is
**hashed (SHA-256) on your device** before it is sent. The app never gives the software your name,
email or any account (there is none).

**What is never in these counts:** your symptoms, pain scores, medication, pressure readings, pressure
history, location or city, or anything you typed. The code has no way to attach such data to an event.

The app does not track you: it does not combine this data with data from other companies and does not
show ads. TelemetryDeck's own practices (where its servers are, how long it keeps data) are described
at telemetrydeck.com.

### 7. Subscriptions

In the current version the subscription screen is switched off. If it is switched on in a future
version, purchases, free trials, renewals and refunds are handled by **Apple** through the App Store.
BaroGuard does not see your card or Apple ID. It only learns, through Apple's StoreKit, whether you have
an active subscription so it can unlock the features. You manage or cancel a subscription in your Apple
ID settings. Apple's standard terms apply (see our Terms: [TERMS URL]).

### 8. Your controls

In **Settings ▸ Your data**:

- **Export my data** creates a JSON file with everything, and two CSV files (symptom logs and pressure
  history), which you can share or save. The temporary copies are deleted when you close the screen.
  The files contain your health notes, so share them carefully.
- **Reset symptom history** deletes all of your symptom logs and keeps everything else.
- **Delete all data** deletes your symptom logs, pressure history, cached forecast, chosen city and all
  app settings, and shows the introduction again. It also stops the TelemetryDeck software and clears the
  information it keeps on your device in the app's storage (the list of days the app was used and the
  session timings described in section 6; the session timings may still be held in memory and saved
  again until the app is next opened). Two things are deliberately **kept**: your
  choice to turn analytics off (otherwise the app would start counting again without you asking) and the
  "already sent" markers for subscription events (otherwise an existing subscriber would be counted
  again). The small Apple Weather attribution image and link are also kept; they contain no personal
  information. If analytics is still on, the TelemetryDeck software starts again the next time the app
  sends a count.
- Deleting the app removes its data from your device. Backups you made earlier still contain it until you
  delete those backups.
- You can withdraw location permission in iOS Settings.

What Delete all data cannot do: it cannot remove counts that TelemetryDeck has already received, because
they are anonymous and not linked to you; and it cannot remove the TelemetryDeck software's own cache file
of counts that were waiting to be sent, because the software offers no way for an app to delete it. That
file holds only event names and the device information listed in section 6 (no health data), and it is
removed when you delete the app. If analytics is on, those waiting counts are sent the next time the
software starts; if you turned analytics off, they are never sent.

### 9. Other points

- BaroGuard has no advertising, no social sharing, no account and no third-party crash-reporting
  software.
- The app downloads the Apple Weather logo from Apple's servers to display it. This request contains no
  personal information from you beyond what any network request reveals (such as your IP address to
  Apple).
- We may update this policy. The2026-10-13 the top changes when we do.

### 10. Not a medical device

BaroGuard does not diagnose, treat or predict any medical condition and gives no medical advice. It
shows air-pressure readings and your own notes. For health questions, talk to a qualified professional.

### 11. Contact

ngothaibao3012@gmail.com

---

## Tiếng Việt

**Ngày có hiệu lực:** 2026-10-13
**Liên hệ:** ngothaibao3012@gmail.com

BaroGuard hiển thị áp suất không khí nơi bạn ở và cho phép bạn ghi lại cảm giác của mình, để bạn có thể
xem hai thứ này cạnh nhau. Trang này giải thích ứng dụng làm gì với thông tin của bạn.

### 1. Tóm tắt

- Ghi chú triệu chứng của bạn chỉ nằm trên iPhone của bạn. BaroGuard không có tài khoản, không có máy
  chủ riêng và không đồng bộ ghi chú của bạn lên đám mây.
- Để hiển thị áp suất không khí, ứng dụng gửi một vị trí **gần đúng** tới Apple Weather.
- Nếu bạn tìm một thành phố, nội dung bạn gõ sẽ được gửi tới Apple Maps.
- Ứng dụng đếm một vài sự kiện ẩn danh (ví dụ "ứng dụng đã được mở") thông qua dịch vụ TelemetryDeck,
  kèm thông tin cơ bản về thiết bị và mức độ thường xuyên, thời gian dùng ứng dụng. Bạn có thể tắt bất cứ lúc nào. Các số đếm này không bao giờ chứa
  triệu chứng, lịch sử áp suất hay vị trí của bạn.
- Bạn có thể xuất toàn bộ dữ liệu hoặc xóa toàn bộ dữ liệu trong Cài đặt.
- BaroGuard không phải là thiết bị y tế (xem mục 10).

### 2. Ứng dụng lưu gì trên thiết bị của bạn

| Nội dung                       | Chi tiết                                                                                                                          |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| Nhật ký triệu chứng            | Thời gian, mức bạn cảm thấy (ổn / nhẹ / đau / phải nằm nghỉ) và, nếu bạn thêm, điểm đau từ 1 đến 10 và thuốc bạn đã dùng.         |
| Lịch sử áp suất                | Các số đo áp suất theo giờ mà ứng dụng đã lấy về, và số đo từ khí áp kế của điện thoại nếu máy có.                                |
| Cài đặt và trạng thái ứng dụng | Đơn vị áp suất, thành phố bạn chọn, việc bạn đã xem xong phần giới thiệu chưa, công tắc thống kê ẩn danh và một vài dấu "đã làm". |
| Ghi nhận nguồn thời tiết       | Logo Apple Weather và liên kết pháp lý mà Apple yêu cầu ứng dụng phải hiển thị.                                                   |

Thông tin này chỉ được lưu trên thiết bị của bạn. Nếu bạn sao lưu iPhone (lên iCloud hoặc vào máy tính),
dữ liệu của ứng dụng nằm trong bản sao lưu đó, vì iOS sao lưu theo cách này. Bạn kiểm soát việc sao lưu
trong Cài đặt iOS và Finder. BaroGuard không tải dữ liệu của bạn lên bất kỳ máy chủ nào và không đồng bộ
giữa các thiết bị.

### 3. Vị trí → Apple Weather

Nếu bạn cho phép truy cập vị trí (khi đang dùng ứng dụng), ứng dụng làm tròn vị trí của bạn tới **0,1 độ,
khoảng 10 km**, rồi gửi vị trí đã làm tròn đó tới **Apple Weather (WeatherKit)** để lấy áp suất hiện tại
và dự báo. Vị trí chính xác không được gửi. Nếu muốn, bạn có thể chọn một thành phố thay vì cho phép vị
trí. Cách Apple xử lý yêu cầu này được mô tả trong tài liệu quyền riêng tư của chính Apple. Ứng dụng không
gửi vị trí của bạn cho nhà phát triển hay cho dịch vụ thống kê.

### 4. Tìm thành phố → Apple Maps

Khi bạn gõ vào ô tìm thành phố, nội dung bạn gõ được gửi tới **Apple Maps** (`MKLocalSearchCompleter`) để
gợi ý địa điểm. Khi bạn chọn một gợi ý, ứng dụng hỏi Apple Maps (`MKLocalSearch`) vị trí của đúng địa điểm
đó. Nội dung gõ không được gửi đi nơi nào khác. Ứng dụng có thông báo điều này ngay trên màn hình tìm kiếm.

### 5. Khí áp kế của điện thoại

Trên iPhone có khí áp kế, ứng dụng đọc nó (khi bạn cho phép "Chuyển động & thể chất") để hiển thị áp suất
tại điện thoại của bạn. Số đo này chỉ nằm trên thiết bị.

### 6. Thống kê sử dụng ẩn danh (TelemetryDeck)

Ứng dụng dùng **TelemetryDeck**, một dịch vụ thống kê chú trọng quyền riêng tư, để biết những phần nào của
ứng dụng được dùng. Tính năng này **bật theo mặc định**. Số đếm đầu tiên có thể được gửi ngay trong lúc bạn
xem phần giới thiệu. Bạn có thể tắt trong **Cài đặt ▸ Dữ liệu của bạn ▸ Chia sẻ dữ liệu sử dụng ẩn danh**;
sau đó sẽ không có gì được gửi nữa. Tắt chỉ dừng việc gửi từ lúc đó; nó không xóa các số đếm đã được nhận.

**Các sự kiện duy nhất ứng dụng có thể gửi** (mỗi sự kiện chỉ là tên của nó, không kèm thông tin nào khác):

| Sự kiện                  | Được gửi khi                                                                                           |
| ------------------------ | ------------------------------------------------------------------------------------------------------ |
| `opened_app`             | Ứng dụng được mở lên màn hình, tối đa một lần mỗi 30 phút                                              |
| `completed_onboarding`   | Bạn xem xong phần giới thiệu                                                                           |
| `first_log`              | Bạn lưu nhật ký triệu chứng đầu tiên của mình                                                          |
| `viewed_forecast`        | Bạn mở một ngày trong dải 7 ngày, hoặc dải này nằm trên màn hình một lúc (một lần mỗi lần mở app)      |
| `viewed_history`         | Bạn mở tab Lịch sử (một lần mỗi lần mở app)                                                            |
| `viewed_pattern`         | Có định nghĩa trong ứng dụng nhưng **không được gửi** ở phiên bản này                                  |
| `started_trial`          | Chỉ khi màn hình đăng ký được bật ở phiên bản sau: bạn bắt đầu dùng thử miễn phí (một lần)             |
| `converted_subscription` | Chỉ khi màn hình đăng ký được bật ở phiên bản sau: bản dùng thử chuyển thành đăng ký trả phí (một lần) |

**Phần mềm TelemetryDeck tự thêm vào** mỗi số đếm. Danh sách này được đọc từ mã nguồn của phần mềm (phiên
bản 2.14.2), nên đây là những gì thiết bị của bạn gửi đi:

- _Ứng dụng và thiết bị:_ phiên bản và số build của ứng dụng; phiên bản iOS; mẫu máy, kiến trúc chip và
  nền tảng; kích thước, tỷ lệ và hướng màn hình; việc ứng dụng là bản TestFlight, App Store, gỡ lỗi hay
  trình mô phỏng; tên và phiên bản của phần mềm TelemetryDeck.
- _Ngôn ngữ và cài đặt:_ ngôn ngữ, khu vực và vùng miền (locale); múi giờ; giao diện sáng hoặc tối; hướng
  bố cục (trái sang phải hoặc phải sang trái); cỡ chữ; và các công tắc trợ năng: giảm chuyển động, chữ
  đậm, đảo ngược màu, tăng độ tương phản màu hệ thống, giảm độ trong suốt, phân biệt không dựa vào màu.
- _Ngày và giờ:_ ngày trong tháng, thứ trong tuần, ngày trong năm, tuần trong năm, tháng, quý, có phải
  cuối tuần hay không, và giờ trong ngày.
- _Các trường lịch sử sử dụng:_ ngày của phiên đầu tiên, số ngày đã dùng ứng dụng (tổng và trong 30 ngày
  gần nhất), tổng số phiên, độ dài phiên trung bình và phiên trước đó (tính bằng giây). Phần mềm luôn có
  các trường này. BaroGuard tắt cài đặt "thống kê phiên" của phần mềm, nhưng phần mềm vẫn giữ danh sách các
  ngày ứng dụng được dùng và một bộ đếm thời gian ứng dụng đang mở, trong vùng lưu trữ riêng của nó trên
  thiết bị của bạn, nên các con số này có thể là số thật. ("Ngày phiên đầu tiên" không được ghi lại trong
  cấu hình này và chỉ đơn giản là ngày của số đếm đó.) Đây là những con số về mức độ thường xuyên và thời
  gian dùng ứng dụng; chúng không nói gì về bạn hay sức khỏe của bạn.

**Một mã định danh ẩn danh.** Để đếm mỗi người một lần, phần mềm dùng "mã định danh dành cho nhà cung cấp"
của iOS (dùng chung cho mọi ứng dụng của nhà phát triển này trên thiết bị của bạn, và không phải mã định
danh quảng cáo). Mã này được **băm (SHA-256) ngay trên thiết bị** trước khi gửi. Ứng dụng không bao giờ đưa
cho phần mềm tên, email hay tài khoản của bạn (ứng dụng không có tài khoản).

**Những gì không bao giờ có trong các số đếm này:** triệu chứng, điểm đau, thuốc, số đo áp suất, lịch sử
áp suất, vị trí hay thành phố, hoặc bất cứ điều gì bạn đã gõ. Mã nguồn không có cách nào đính kèm những dữ
liệu đó vào một sự kiện.

Ứng dụng không theo dõi bạn: không kết hợp dữ liệu này với dữ liệu của công ty khác và không hiển thị quảng
cáo. Cách làm riêng của TelemetryDeck (máy chủ ở đâu, lưu dữ liệu bao lâu) được mô tả tại telemetrydeck.com.

### 7. Đăng ký (subscription)

Ở phiên bản hiện tại, màn hình đăng ký đang tắt. Nếu được bật ở phiên bản sau, việc mua, dùng thử miễn phí,
gia hạn và hoàn tiền do **Apple** xử lý qua App Store. BaroGuard không nhìn thấy thẻ hay Apple ID của bạn.
Ứng dụng chỉ biết, thông qua StoreKit của Apple, bạn có đang đăng ký hay không để mở khóa tính năng. Bạn
quản lý hoặc hủy đăng ký trong cài đặt Apple ID. Áp dụng điều khoản tiêu chuẩn của Apple (xem
Điều khoản: [TERMS URL]).

### 8. Quyền kiểm soát của bạn

Trong **Cài đặt ▸ Dữ liệu của bạn**:

- **Xuất dữ liệu của tôi** tạo một tệp JSON chứa mọi thứ và hai tệp CSV (nhật ký triệu chứng và lịch sử áp
  suất) để bạn chia sẻ hoặc lưu lại. Bản sao tạm được xóa khi bạn đóng màn hình. Các tệp chứa ghi chú sức
  khỏe của bạn, vì vậy hãy chia sẻ cẩn thận.
- **Đặt lại lịch sử triệu chứng** xóa toàn bộ nhật ký triệu chứng và giữ nguyên mọi thứ khác.
- **Xóa toàn bộ dữ liệu** xóa nhật ký triệu chứng, lịch sử áp suất, dự báo đã lưu, thành phố đã chọn và mọi
  cài đặt của ứng dụng, rồi hiển thị lại phần giới thiệu. Nó cũng dừng phần mềm TelemetryDeck và xóa thông
  tin phần mềm này giữ trên thiết bị của bạn trong vùng lưu trữ của ứng dụng (danh sách các ngày đã dùng ứng dụng và
  thời lượng phiên nêu ở mục 6; thời lượng phiên có thể vẫn còn trong bộ nhớ và được lưu lại cho tới lần
  mở ứng dụng kế tiếp). Có hai thứ được **giữ lại có chủ đích**: lựa chọn
  tắt thống kê của bạn (nếu không ứng dụng sẽ đếm lại mà bạn không yêu cầu) và các dấu "đã gửi" của sự kiện
  đăng ký (nếu không người đã đăng ký sẽ bị đếm lại). Ảnh và liên kết ghi nhận nguồn Apple Weather nhỏ cũng
  được giữ lại; chúng không chứa thông tin cá nhân. Nếu thống kê vẫn bật, phần mềm TelemetryDeck sẽ khởi
  động lại vào lần tiếp theo ứng dụng gửi một số đếm.
- Xóa ứng dụng sẽ xóa dữ liệu của nó khỏi thiết bị. Các bản sao lưu bạn đã tạo trước đó vẫn chứa dữ liệu
  cho đến khi bạn xóa các bản sao lưu đó.
- Bạn có thể thu hồi quyền vị trí trong Cài đặt iOS.

Những gì Xóa toàn bộ dữ liệu không làm được: không thể xóa các số đếm TelemetryDeck đã nhận, vì chúng ẩn
danh và không gắn với bạn; và không thể xóa tệp bộ nhớ đệm riêng của phần mềm TelemetryDeck chứa các số đếm
đang chờ gửi, vì phần mềm không cung cấp cách nào để ứng dụng xóa nó. Tệp đó chỉ chứa tên sự kiện và thông
tin thiết bị nêu ở mục 6 (không có dữ liệu sức khỏe), và sẽ bị xóa khi bạn xóa ứng dụng. Nếu thống kê đang
bật, các số đếm đang chờ đó sẽ được gửi vào lần phần mềm khởi động tiếp theo; nếu bạn đã tắt thống kê, chúng
không bao giờ được gửi.

### 9. Các điểm khác

- BaroGuard không có quảng cáo, không chia sẻ mạng xã hội, không có tài khoản và không dùng phần mềm báo
  lỗi của bên thứ ba.
- Ứng dụng tải logo Apple Weather từ máy chủ của Apple để hiển thị. Yêu cầu này không chứa thông tin cá
  nhân nào từ bạn ngoài những gì mọi yêu cầu mạng đều tiết lộ (ví dụ địa chỉ IP của bạn với Apple).
- Chúng tôi có thể cập nhật chính sách này. Ngày có hiệu lực ở đầu trang sẽ thay đổi khi đó.

### 10. Không phải thiết bị y tế

BaroGuard không chẩn đoán, không điều trị và không dự đoán bất kỳ tình trạng bệnh nào, và không đưa ra lời
khuyên y tế. Ứng dụng chỉ hiển thị số đo áp suất không khí và ghi chú của chính bạn. Với các câu hỏi về sức
khỏe, hãy trao đổi với chuyên gia có chuyên môn.

### 11. Liên hệ

ngothaibao3012@gmail.com
