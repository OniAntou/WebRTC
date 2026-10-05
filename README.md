# WebRTC

Lab thực hành WebRTC & Network Protocol: Client/Server SDP Architecture, P2P Chat với DataChannel.

## Nội dung

- `AnhTu.html` — Trang lab duy nhất, gồm 3 tab:
  1. Kiến trúc & phân tách SDP
  2. Phòng thực hành P2P Chat (TCP-like / UDP-like, Burst Stream, RTT)
  3. Cơ chế Signaling tự động trong thực tế

## Chạy local

Mở bằng Web Server (không mở `file://` trực tiếp để tránh lỗi WebRTC):

- VSCode + extension Live Server, hoặc:
- `npx serve .`

Sau đó mở 2 tab / 2 máy cùng mạng LAN để handshake OFFER/ANSWER.

## Handshake nhanh

1. Tab A: `1. Tạo OFFER Signal` → Copy.
2. Tab B: dán vào Signal Nhận → `2. Chấp Nhận & Kết Nối` → Copy ANSWER.
3. Tab A: dán ANSWER → `Chấp Nhận & Kết Nối`.
