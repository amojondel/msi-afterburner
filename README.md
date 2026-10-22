download msi afterburner: https://www.msi.com/Landing/afterburner/graphics-cards
download hwinfo: https://www.hwinfo.com/files/hwi64_854.exe
فارسی
## نصب

1. ZIP را کامل Extract کن.
2. بازی‌ها را ببند.
3. `Install-RTSS-PositionFix.cmd` را اجرا کن و در پنجرهٔ UAC روی Yes بزن.
4. فایل `RTSS-position-fix.log` را بررسی کن؛ اگر با `SUCCESS` شروع شود، تنظیم نصب شده است.
5. RTSS را باز نگه دار، یک بازی را باز و بسته کن و دوباره باز کن تا ثابت‌ماندن جای اورلی را بررسی کنی.

اسکریپت پیش از تغییر، از پروفایل RTSS نسخهٔ پشتیبان می‌گیرد. برای بازگردانی، فایل `RTSS-Global.before-position-fix` را به مسیر `C:\Program Files (x86)\RivaTuner Statistics Server\Profiles\Global` برگردان و RTSS را دوباره اجرا کن.

## فعال‌کردن سنسورها

1. HWiNFO، MSI Afterburner و RTSS را نصب کن.
2. HWiNFO را باز کن و در پنجرهٔ اصلی وارد `Settings` شو. گزینهٔ `Shared Memory Support` را روشن و تنظیمات را ذخیره کن. اگر HWiNFO در حالت Sensors-only اجرا شده، روی آیکونش کنار ساعت ویندوز راست‌کلیک کن و از آنجا `Settings` را باز کن.
3. در تنظیمات HWiNFO، `Auto Start` را فعال کن تا همراه ورود به ویندوز اجرا شود. حالت `Sensors-only` و `Minimize Sensors on Startup` را هم فعال کن تا سنسورها بدون پنجرهٔ بزرگ باز شوند. پنجرهٔ Sensors را نبند؛ آن را Minimize کن تا HWiNFO در پس‌زمینه/کنار ساعت فعال بماند و داده به MSI برسد.
4. MSI Afterburner و RTSS را هم باز نگه دار؛ برای نمایش اورلی هر سه برنامه باید در حال اجرا باشند.
5. از پروفایل MSI داخل بسته استفاده کن. پیش از جایگزینی فایل هم‌نام در پوشهٔ `MSI Afterburner\Profiles`، از فایل قبلی نسخهٔ پشتیبان بگیر.
6. در MSI Afterburner به `Settings > Monitoring` برو، سنسورهای موردنیاز را انتخاب کن و `Show in On-Screen Display` را فعال کن.
7. برای هر دیسک، سنسور همان دستگاه را انتخاب کن و نام گروه را با پارتیشنش بنویس؛ مثلاً `SSD3 (D:)`. پروفایل ردیف‌های SSD1 تا SSD4 را دارد. دما فقط وقتی نمایش داده می‌شود که خود دیسک و کنترلرش آن را گزارش کنند.

## پاور و سازگاری

ولتاژهای +3.3V، +5V و +12V فقط در صورت گزارش مادربرد نمایش داده می‌شوند. توان، جریان، دما و دور فن پاور فقط با پاور و افزونهٔ سازگار در دسترس هستند؛ UPS با PSU فرق دارد. فهرست سنسورها به سخت‌افزار، درایور و کنترلر ذخیره‌سازی بستگی دارد. اگر سنسوری در فهرست نیست، آن قطعه یا نرم‌افزار داده‌اش را ارائه نمی‌کند.

English
## Installation

1. Extract the entire ZIP file.
2. Close any running games.
3. Run `Install-RTSS-PositionFix.cmd` and click "Yes" in the UAC prompt.
4. Check the `RTSS-position-fix.log` file; if it begins with `SUCCESS`, the fix has been installed.
5. Keep RTSS running, then open and close a game (and open it again) to verify that the overlay position remains fixed.

The script creates a backup of your RTSS profile before making any changes. To revert, move the `RTSS-Global.before-position-fix` file back to `C:\Program Files (x86)\RivaTuner Statistics Server\Profiles\Global` and restart RTSS.

## Enabling Sensors

1. Install HWiNFO, MSI Afterburner, and RTSS.
2. Open HWiNFO and go to `Settings` from the main window. Enable `Shared Memory Support` and save your settings. If HWiNFO is running in "Sensors-only" mode, right-click its icon near the Windows system tray (clock) and access `Settings` from there.
3. In the HWiNFO settings, enable `Auto Start` so it launches when you log into Windows. Also, enable `Sensors-only` and `Minimize Sensors on Startup` to ensure the sensors launch without opening a large window. Do not close the Sensors window; minimize it instead so that HWiNFO remains active in the background (near the system tray) and continues sending data to MSI Afterburner.
4. Keep both MSI Afterburner and RTSS running; all three applications must be active for the overlay to display.
5. Use the MSI profile included in the package. Before replacing the file of the same name in the `MSI Afterburner\Profiles` folder, create a backup of the existing file.
6. In MSI Afterburner, go to `Settings > Monitoring`, select the required sensors, and enable `Show in On-Screen Display`.
7. For each disk, select the corresponding sensor and set the group name to match its partition (e.g., `SSD3 (D:)`). The profile includes entries for SSD1 through SSD4. Temperature data is displayed only if the disk itself and its controller report it.

## Power Supply and Compatibility

The +3.3V, +5V, and +12V voltage rails are displayed only if reported by the motherboard. Power, current, temperature, and fan speed for the power supply unit (PSU) are available only when using a compatible PSU and the appropriate extension; note that a UPS is distinct from a PSU. The list of available sensors depends on your hardware, drivers, and storage controller. If a sensor does not appear in the list, it means the respective component or software is not providing that data.
