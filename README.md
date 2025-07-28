# 🌊 SURF — Simulated Usability and Rating Framework

**SURF** is a Rust library that helps Yew developers build better web UIs by combining:

- ✅ Prebuilt, configurable **Yew components**
- 📊 Automated **usability summaries** based on simulated user behavior

You can use SURF to quickly build a layout, run a local simulation, and get feedback like:
- Which buttons users are likely to click
- Which areas of the UI are less intuitive
- Overall usability ratings

---

## 🧭 What SURF Does

1. **Assemble a layout** using SURF’s ready-made Yew templates
2. **Run a simulation** to predict how users will interact
3. **Get a summary report** with clickability, usability scores, and design tips

---

## 🚀 Example (coming soon)

```rust
use surf::templates::LoginForm;
use surf::simulate;

let ui = LoginForm::new().with_remember_me(true);
let report = simulate(ui);

println!("{}", report.summary());
