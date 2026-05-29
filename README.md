
# 🐧
---
```c
typedef enum {
    MODE_STUDYING,
    MODE_BUILDING
} OperationalMode;

struct EmbeddedState {
    const char *dialogue;
    const char *current_focus;
    void *system_boundary;
};

struct EmbeddedState init_system_state(OperationalMode mode) {
    struct EmbeddedState state = {
        .dialogue = "Nothing goes with a percocet like some good air conditioning, ya know?",
        .system_boundary = (void *)0xC0000000
    };

    if (mode == MODE_STUDYING) {
        state.current_focus = "bachelor of being a nerd";
    } else {
        state.current_focus = "testudo like the roman military formation which is pretty neat but I try not to think about parthian campaigns and caligula and stuff like that";
    }

    return state;
}
```

---
### Contact

📧 [sub0xdai@proton.me](mailto:sub0xdai@proton.me)










                        
