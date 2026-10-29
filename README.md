# Bonk3rs

Game hành động 2D góc nhìn từ trên xuống, làm bằng **Unity 6 (6000.2.13f1)** với Universal Render Pipeline (2D). Repo này chứa **bản build cho Windows**, không chứa source project Unity.

## Gameplay

- Chiến đấu qua nhiều màn chơi (Map 1 → Map 2 → Map 3), mỗi màn có quái cận chiến, quái tầm xa và bẫy xuất hiện quanh người chơi.
- Cuối màn là trận đánh boss với nhiều chiêu thức: lướt tấn công (dash), đuổi đánh, tấn công diện rộng và bắn đạn đuổi.
- Hạ quái để nhặt vàng và bình máu.
- Dùng vàng để nâng cấp chỉ số (sát thương, tốc độ đánh, tầm đánh) và thu thập thêm vũ khí.

## Cách chạy

**Yêu cầu:** Windows 64-bit, card đồ họa hỗ trợ DirectX 11/12.

1. Clone repo:
   ```sh
   git clone <url-repo> Bonk3rs
   ```
2. Mở thư mục `Bonk3rs` và chạy `Game_1.exe`.

Giữ nguyên cấu trúc thư mục — `Game_1.exe` cần các file `UnityPlayer.dll`, `Game_1_Data/`, `MonoBleedingEdge/` và `D3D12/` nằm cùng chỗ.

## Cấu trúc thư mục

| Đường dẫn | Mô tả |
| --- | --- |
| `Game_1.exe` | File chạy game |
| `Game_1_Data/` | Dữ liệu game: scene, asset, assembly đã biên dịch |
| `UnityPlayer.dll` | Runtime của Unity |
| `MonoBleedingEdge/` | Runtime Mono cho script C# |
| `D3D12/` | Thư viện Direct3D 12 |
| `UnityCrashHandler64.exe` | Trình báo lỗi khi game crash |
| `Game_1_BurstDebugInformation_DoNotShip/` | Thông tin debug của Burst — không cần khi phát hành |
