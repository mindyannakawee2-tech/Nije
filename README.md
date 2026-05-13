<img src="banner.png" width="1000">

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
>QOL
since there is some memory leaks when you use C++ so I'd recommened doing this instead
```cpp
texture.reset(Content::Load<Texture2D>("path/to/image", renderer.get()));
object = std::make_unique<Object2D>(texture.get(), renderer.get());
```
