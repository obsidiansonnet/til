# `position: absolute` Ignores Its Parent's Padding

Unlike `static`, `relative`, and `sticky` elements—which remain in flow and resolve against their parent's **content box**—`position: absolute` elements are taken out of flow and resolve their inset and percentage values against their Containing Block's **padding box**.

As a result, `top: 0` sits flush against the inner border, and `width: 100%` spans the full content + padding width.