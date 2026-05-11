# Nije
A Powerful Godot-Based Framework for C++

# API
>Load Contents
```cpp
// Texture2D
Content::Load<Texture2D>("path/to/image", renderer);
// Audio
Content::Load<Audio>("path/to/audio");
```
>Contents usage
```cpp
// Texture2D
Nije::Draw(renderer, texture, srcRect, destRect);
object2d = new Object2D(texture, renderer);

// Audio
audioName->Play(bool Looped);
```
