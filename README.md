## Hey there I'm Khaled

CS student · Software & Systems Engineer  
I write Rust, C/C++, and Python - from kernel-level primitives to backend systems.  
Driven by the belief that every abstraction has a cost, and every cost can be measured.

````rust
#![allow(unused_variables, dead_code)]
use core::arch::asm;
use core::hint::{black_box, unreachable_unchecked};
use core::ptr;

// I am the bone of my Pointer.
pub struct UnlimitedOptimizationWorks;

pub trait Bone {
    type Body;   // Assembly is my body.
    type Blood;  // Thermal-Throttling is my blood.
}

impl Bone for UnlimitedOptimizationWorks {
    type Body  = asm!();
    type Blood = f32; // heat
}

impl UnlimitedOptimizationWorks {
    #[inline(always)]
    pub unsafe fn trace_circuit<T>(pointer: *const T) -> ! {
        // I have unrolled over a thousand loops.
        (0..1024u16).for_each(|i| { black_box(i); });

        // Unaware of Branch Misprediction. Nor aware of Cache Misses.
        if black_box(false)           { unreachable_unchecked(); }
        if pointer == ptr::null::<T>() { unreachable_unchecked(); }

        // Withstood Undefined Behavior to reach Zero-Latency.
        let _ = ptr::read_volatile(pointer);

        // I have no regrets. This is the only path.
        asm!(
            "/* As I Pray — Unlimited Optimization Works! */",
            options(noreturn, nostack)
        );
    }
}
````
---

### Current work
- **[Vulnera](https://github.com/Vulnera-rs)** — security framework  
- **[gthreads](https://github.com/k5602/gthreads)** — threading primitives  
- **[RiftSiege](https://github.com/k5602/rift_siege)** — game project  
- **[CoursePilot](https://github.com/k5602/course_pilot)** — academic tooling  
- Active OSS contributor

> *"Withstood Undefined Behavior to reach Zero-Latency."*
