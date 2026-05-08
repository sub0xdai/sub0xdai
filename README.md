
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
        .system_boundary = (void *)0xC0000000
    };

    if (mode == MODE_STUDYING) {
        state.current_focus = "Bachelor of Cybersecurity";
        state.dialogue = "Nothing goes with a percocet like some good air conditioning, ya know?";
    } else {
        state.current_focus = "Testudo: Risk Management Perp Trading App";
        state.dialogue = "Building agentic flows.";
    }

    return state;
}
```

---
### Contact

📧 [sub0xdai@proton.me](mailto:sub0xdai@proton.me)










                        
