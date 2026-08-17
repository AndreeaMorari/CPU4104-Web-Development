# CPU4104-Web-Development - G268784 

-- INDEX CODE

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Home | A Quiet Haven</title>
    <meta
      name="description"
      content="A low-stimulation digital sanctuary — ambient soundscapes, anonymous letters, a curated reading room, and the slow art of handwritten correspondence."
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAVIGATION ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html" class="active">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <!-- ================= HERO ================= -->
      <section class="hero">
        <img
          class="hero-watermark"
          src="media/logo-seal.png"
          alt=""
          aria-hidden="true"
        />
        <div class="container">
          <span class="eyebrow">A Digital Sanctuary</span>
          <h1>
            A quiet place to land, when the world has been loud for too long.
          </h1>
          <p class="literary-italic measure-tight">
            For anyone carrying loneliness, grief, heartbreak, or a week that
            simply asked too much — held gently here through ambient
            soundscapes, anonymous letters, and the slow, deliberate art of
            writing by hand.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <!-- ================= OPEN A LETTER ================= -->
      <section>
        <div class="container">
          <div class="section-head">
            <span class="eyebrow">Anonymous Community Letters</span>
            <h2>Open a Letter</h2>
            <p>
              A short, anonymous message left behind by a stranger, for whoever
              arrives next and needs it. Take as many as you like — they cost
              nothing.
            </p>
          </div>
          <div class="card card--solo">
            <p
              class="literary-italic"
              id="letter-quote"
              style="font-size: 1.15rem"
            >
              &ldquo;You do not have to carry the whole weight of the sky today.
              Soften your shoulders, breathe, and know that you are allowed to
              simply rest.&rdquo;
            </p>
            <p class="card-tag" id="letter-byline">— A stranger, somewhere</p>
            <button type="button" class="btn" id="open-letter-btn">
              Open Another Letter
            </button>
          </div>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <!-- ================= LEAVE A NOTE ================= -->
      <section>
        <div class="container">
          <div class="section-head">
            <span class="eyebrow">Leave a Note</span>
            <h2>Write a Quiet Word for the Next Visitor</h2>
            <p>
              Your message is added anonymously to the sanctuary, ready for a
              stranger to open on the evening they need it most.
            </p>
          </div>

          <div
            id="note-success"
            class="form-success"
            role="status"
            style="max-width: 640px"
          >
            Thank you. Your words have been gently placed in the sanctuary for
            someone else to find.
          </div>

          <form class="card card--solo" id="note-form" novalidate>
            <div class="field">
              <label for="note-message">Your Message</label>
              <textarea
                id="note-message"
                name="message"
                maxlength="400"
                placeholder="Leave a short note of encouragement, comfort, or quiet honesty..."
              ></textarea>
            </div>
            <div class="field">
              <label for="note-from"
                >Sign As (optional — leave blank to stay anonymous)</label
              >
              <input
                type="text"
                id="note-from"
                name="from"
                placeholder="e.g. A stranger in London"
              />
            </div>
            <button type="submit" class="btn">Leave a Note</button>
          </form>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <!-- ================= NEWSLETTER ================= -->
      <section>
        <div class="container">
          <div class="section-head">
            <span class="eyebrow">The Digital Newsletter</span>
            <h2>Letters, Delivered to Your Inbox</h2>
            <p>
              Choose the rhythm that suits your season. Nothing is ever urgent,
              and every issue can be left unopened without consequence.
            </p>
          </div>

          <div
            id="newsletter-success"
            class="form-success"
            role="status"
            style="max-width: 640px"
          ></div>

          <form class="card card--solo" id="newsletter-form" novalidate>
            <fieldset style="border: none; padding: 0; margin: 0 0 0.4rem">
              <legend class="form-label" style="padding: 0">
                Choose Your Rhythm
              </legend>
              <div class="radio-row">
                <label class="radio-pill"
                  ><input
                    type="radio"
                    name="tier"
                    value="Daily Reflections"
                    checked
                  />Daily Reflections</label
                >
                <label class="radio-pill"
                  ><input
                    type="radio"
                    name="tier"
                    value="Weekly Solace"
                  />Weekly Solace</label
                >
                <label class="radio-pill"
                  ><input
                    type="radio"
                    name="tier"
                    value="Monthly Healing"
                  />Monthly Healing</label
                >
              </div>
            </fieldset>
            <div class="field">
              <label for="newsletter-email">Email Address</label>
              <input
                type="email"
                id="newsletter-email"
                name="email"
                placeholder="you@example.com"
              />
            </div>
            <button type="submit" class="btn">Subscribe</button>
          </form>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <!-- ================= READING ROOM ================= -->
      <section>
        <div class="container">
          <div class="section-head">
            <span class="eyebrow">Curated Reading Room</span>
            <h2>Recommended Reading for the Mind</h2>
            <p>
              A small, handpicked shelf. Nothing here promises to fix you —
              these are simply books that have quietly kept people company
              through anxiety, trauma, boundaries, and grief.
            </p>
          </div>
          <!-- FLAG: the spec calls for outbound retailer links but names no retailer, so all five point to Amazon UK product pages by ISBN. Say the word if you would rather they went to Bookshop.org, Waterstones, or your own affiliate links. -->
          <div class="grid">
            <div class="card">
              <span class="card-tag">On Everyday Coping</span>
              <h3>Why Has Nobody Told Me This Before?</h3>
              <span class="book-meta">Dr Julie Smith</span>
              <p>
                Practical therapy tools for low moods, motivation, and anxiety,
                written in small chapters you can read on a bad day without
                needing much of yourself.
              </p>
              <a
                class="btn"
                href="https://www.amazon.co.uk/dp/0241529719"
                target="_blank"
                rel="noopener"
                >View Book</a
              >
            </div>
            <div class="card">
              <span class="card-tag">On Acceptance</span>
              <h3>The Happiness Trap</h3>
              <span class="book-meta">Russ Harris</span>
              <p>
                An accessible introduction to Acceptance and Commitment Therapy,
                and a gentle argument that chasing happiness is often what costs
                us it.
              </p>
              <a
                class="btn"
                href="https://www.amazon.co.uk/dp/184529825X"
                target="_blank"
                rel="noopener"
                >View Book</a
              >
            </div>
            <div class="card">
              <span class="card-tag">On Boundaries</span>
              <h3>Set Boundaries, Find Peace</h3>
              <span class="book-meta">Nedra Glover Tawwab</span>
              <p>
                A grounded, unsentimental guide to reclaiming yourself through
                boundaries — including the ones that feel unkind to draw.
              </p>
              <a
                class="btn"
                href="https://www.amazon.co.uk/dp/0349426953"
                target="_blank"
                rel="noopener"
                >View Book</a
              >
            </div>
            <div class="card">
              <span class="card-tag">On Trauma</span>
              <h3>The Body Keeps the Score</h3>
              <span class="book-meta">Bessel van der Kolk</span>
              <p>
                A landmark exploration of how trauma settles into the body as
                well as the mind, and of the many quiet routes back out of it.
              </p>
              <a
                class="btn"
                href="https://www.amazon.co.uk/dp/0143127748"
                target="_blank"
                rel="noopener"
                >View Book</a
              >
            </div>
            <div class="card">
              <span class="card-tag">On Staying</span>
              <h3>Reasons to Stay Alive</h3>
              <span class="book-meta">Matt Haig</span>
              <p>
                A tender, short memoir of depression and recovery, written by
                someone who is careful never to pretend the way through was
                tidy.
              </p>
              <a
                class="btn"
                href="https://www.amazon.co.uk/dp/1782116826"
                target="_blank"
                rel="noopener"
                >View Book</a
              >
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>


-- SHOP CODE ##BUY A LETTER

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Buy a Letter | A Quiet Haven</title>
    <meta
      name="description"
      content="Six handwritten letters, each £5, sealed by hand and posted first class — choose a theme, or let fate decide."
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mobile.css" media="(max-width: 899px)" />
    <link rel="stylesheet" href="desktop.css" media="(min-width: 900px)" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAVIGATION ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html" class="active">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">The Letter Marketplace</span>
          <h1>Buy a Letter</h1>
          <p class="literary-italic measure">
            Six handwritten letters, each £5, written in a real hand on real
            paper, sealed in wax, and posted first class. Choose the one that
            fits the season you are in — or let fate decide with the Random
            Letter.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div id="shop-grid" class="product-grid"></div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

  ## SELL A LETTER CODE

  <!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sell a Letter | A Quiet Haven</title>
    <meta
      name="description"
      content="Apply to become one of the writers behind A Quiet Haven's handwritten letters."
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mobile.css" media="(max-width: 899px)" />
    <link rel="stylesheet" href="desktop.css" media="(min-width: 900px)" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAVIGATION ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html" class="active">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">Join Our Writers</span>
          <h1>Sell a Letter</h1>
          <p class="literary-italic measure">
            If you write with care, and you can sit with someone else's
            difficult week without rushing them out of it, we would like to read
            your work. Every application is read by hand.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div
            id="sell-success"
            class="form-success"
            role="status"
            style="max-width: 640px"
          >
            Thank you for your application. We read every submission by hand,
            and will write back within a week.
          </div>

          <form class="card card--solo" id="sell-form" novalidate>
            <div class="field">
              <label for="writer-name">Your Name</label>
              <input
                type="text"
                id="writer-name"
                name="name"
                placeholder="Your full name"
              />
            </div>
            <div class="field">
              <label for="writer-email">Email Address</label>
              <input
                type="email"
                id="writer-email"
                name="email"
                placeholder="you@example.com"
              />
            </div>
            <div class="field">
              <label for="writer-specialty">Writing Specialty</label>
              <select id="writer-specialty" name="specialty">
                <option value="">Choose one...</option>
                <option value="Love">Love</option>
                <option value="Comfort">Comfort</option>
                <option value="Romantic">Romantic</option>
                <option value="Grief &amp; Healing">Grief &amp; Healing</option>
                <option value="Self-Compassion">Self-Compassion</option>
                <option value="Catch-up">Catch-up</option>
              </select>
            </div>
            <div class="field">
              <label for="writer-excerpt">A Short Writing Sample</label>
              <textarea
                id="writer-excerpt"
                name="excerpt"
                placeholder="Share a few sentences of your writing, so we can hear your voice..."
              ></textarea>
            </div>
            <div class="field">
              <span class="form-label" id="writer-photo-hint"
                >Photo or Writing Sample Upload (optional)</span
              >
              <div class="file-row">
                <input
                  type="file"
                  id="writer-photo"
                  name="photo"
                  class="visually-hidden-input"
                  aria-describedby="writer-photo-hint"
                />
                <label for="writer-photo" id="writer-photo-label" class="btn"
                  >Choose a file...</label
                >
              </div>
            </div>
            <button type="submit" class="btn">Submit Application</button>
          </form>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

## DIGITAL LETTERS CODE

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Digital Letter | A Quiet Haven</title>
    <meta
      name="description"
      content="Printable letter templates, archives, and stationery sheets, delivered the moment you need them."
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mobile.css" media="(max-width: 899px)" />
    <link rel="stylesheet" href="desktop.css" media="(min-width: 900px)" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAV ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html" class="active">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">Instant Correspondence</span>
          <h1>Digital Letter</h1>
          <p class="literary-italic measure">
            For the nights when waiting for the post is too long a wait —
            printable templates, archives, and stationery sheets, yours the
            moment you ask for them.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div id="digital-grid" class="product-grid"></div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>


## STATIONARY CODE

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Start a Letter | A Quiet Haven</title>
    <meta
      name="description"
      content="Fine paper, pen and ink, envelopes, and wax seals for beginning your own handwritten correspondence."
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mobile.css" media="(max-width: 899px)" />
    <link rel="stylesheet" href="desktop.css" media="(min-width: 900px)" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAV ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html" class="active">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">The Writing Ritual</span>
          <h1>Start a Letter</h1>
          <p class="literary-italic measure">
            Everything needed to begin your own correspondence — fine paper, a
            pen that rewards a slow hand, envelopes, and wax to seal whatever
            you have finally managed to say.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div id="stationery-grid" class="product-grid"></div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

## CART CODE 

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cart | A Quiet Haven</title>
    <meta
      name="description"
      content="Review your gathered letters and stationery, then release them into the world."
    />
    <link rel="stylesheet" href="style.css" />
    <link rel="stylesheet" href="mobile.css" media="(max-width: 899px)" />
    <link rel="stylesheet" href="desktop.css" media="(min-width: 900px)" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAV ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html">About Us</a>
        <a href="cart.html" class="active"
          >Cart <span class="cart-count">0</span></a
        >
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">Your Selected Reflections</span>
          <h1>Cart</h1>
          <p class="literary-italic measure">
            Everything you have gathered, held quietly here until you are ready
            to send it onward. Nothing expires, and nothing is in a hurry.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div id="cart-empty" class="cart-empty">
            <p class="literary-italic">
              Your cart is quiet right now — nothing has been gathered yet. When
              you are ready, there are letters waiting to be chosen.
            </p>
            <a class="btn" href="shop.html">Browse Letters</a>
          </div>

          <!-- CART -->
          <div id="cart-layout" class="cart-layout">
            <div id="cart-list"></div>

            <div class="cart-summary">
              <h3>Sum of Solace</h3>
              <div class="summary-row">
                <span>Subtotal</span><span id="cart-subtotal">£0.00</span>
              </div>
              <div class="summary-row">
                <span>Delivery</span><span id="cart-shipping">£0.00</span>
              </div>
              <div class="summary-row total">
                <span>Total</span><span id="cart-total">£0.00</span>
              </div>

              <div
                id="checkout-success"
                class="form-success"
                role="status"
                style="margin-top: 1.3rem; margin-bottom: 0"
              >
                Thank you. Your letters are on their way — release into the
                world.
              </div>

              <form id="checkout-form" style="margin-top: 1.4rem" novalidate>
                <div class="field">
                  <label for="checkout-name">Recipient Name</label>
                  <input
                    type="text"
                    id="checkout-name"
                    name="name"
                    placeholder="Full name"
                  />
                </div>
                <div class="field">
                  <label for="checkout-email">Email Address</label>
                  <input
                    type="email"
                    id="checkout-email"
                    name="email"
                    placeholder="you@example.com"
                  />
                </div>
                <div class="field">
                  <label for="checkout-address">Delivery Address</label>
                  <textarea
                    id="checkout-address"
                    name="address"
                    placeholder="Street, city, postcode, country"
                  ></textarea>
                </div>
                <button type="submit" class="btn btn-block">
                  Release Into the World
                </button>
              </form>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

## ABOUT CODE

<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>About Us | A Quiet Haven</title>
    <meta
      name="description"
      content="The story, purpose, and people behind A Quiet Haven — and how to reach us."
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <!-- ================= AMBIENT SOUND PLAYER ================= -->
    <div class="soundbar">
      <span class="soundbar-label">Ambient Sanctuary</span>
      <button type="button" class="sound-btn" data-src="media/rain.mp3">
        Rain
      </button>
      <button type="button" class="sound-btn" data-src="media/storm.mp3">
        Storm
      </button>
      <button type="button" class="sound-btn" data-src="media/ocean.mp3">
        Ocean
      </button>
      <button type="button" class="sound-btn" data-src="media/forest.mp3">
        Forest
      </button>
      <button type="button" class="sound-btn" data-src="media/birds.mp3">
        Birds
      </button>
      <button type="button" class="sound-btn" data-src="media/white-noise.mp3">
        White Noise
      </button>
    </div>

    <!-- ================= FIXED RIGHT SIDEBAR NAVIGATION ================= -->
    <aside class="sidebar">
      <div class="sidebar-brand">
        <img src="media/logo-seal.png" alt="A Quiet Haven wax seal emblem" />
        <div class="name">A Quiet Haven</div>
        <div class="tagline">Sanctuary</div>
      </div>
      <nav>
        <a href="index.html">Home</a>
        <a href="shop.html">Buy a Letter</a>
        <a href="sell.html">Sell a Letter</a>
        <a href="stationery.html">Start a Letter</a>
        <a href="digital.html">Digital Letter</a>
        <a href="about.html" class="active">About Us</a>
        <a href="cart.html">Cart <span class="cart-count">0</span></a>
      </nav>
    </aside>

    <main>
      <section>
        <div class="container">
          <span class="eyebrow">Our Story</span>
          <h1>About Us</h1>
          <p class="literary-italic measure">
            A Quiet Haven began as a single wax-sealed envelope, left on a
            windowsill for a stranger who needed it more than we did. It has
            since grown into a sanctuary for anyone carrying loneliness, grief,
            heartbreak, or anxiety — and for anyone who simply misses being
            written to.
          </p>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div class="grid">
            <div class="card">
              <span class="card-tag">Our Purpose</span>
              <h3>Why We Exist</h3>
              <p>
                The world moves quickly and loudly, and most of what is built
                for it is designed to hold your attention rather than settle it.
                We wanted the opposite: a low-stimulation room with soft sound,
                slow rituals, and nothing flashing for you.
              </p>
              <p>
                Nothing here counts your streak, ranks your progress, or asks
                you to come back tomorrow. Stay as long as it helps, and leave
                without saying goodbye.
              </p>
            </div>
            <div class="card">
              <span class="card-tag">Our Writers</span>
              <h3>Who Writes for You</h3>
              <p>
                Every letter is written by hand, by one of a small group of
                vetted writers chosen for warmth, discretion, and a genuine care
                with words. We read applications individually — never
                automatically — and we would rather grow slowly than lose the
                voice of the thing.
              </p>
              <p>
                If that sounds like your kind of work, the door is open on the
                <a href="sell.html">Sell a Letter</a> page.
              </p>
            </div>
            <div class="card">
              <span class="card-tag">Our Promise</span>
              <h3>Our Promise to You</h3>
              <p>
                Anonymous notes left in the sanctuary are read before they are
                ever shared onward, so that this stays a safe and kind place to
                arrive at on a bad night.
              </p>
              <p>
                We keep only what we need to send you a letter, we never sell
                it, and we never write to you more often than the rhythm you
                chose. A letter should always feel like a gift, never an
                obligation.
              </p>
            </div>
          </div>
        </div>
      </section>

      <div class="ornament" aria-hidden="true">&#10086;</div>

      <section>
        <div class="container">
          <div class="section-head">
            <span class="eyebrow">Reach Us</span>
            <h2>Contact the Sanctuary</h2>
            <p>
              Questions about an order, a letter that went astray, or an
              application in progress — it reaches a real person, and we read
              everything ourselves.
            </p>
          </div>
          <div class="card card--solo">
            <span class="card-tag">Email</span>
            <p>
              <a href="mailto:hello@aquiethaven.co.uk"
                >hello@aquiethaven.co.uk</a
              >
            </p>
            <span class="card-tag">By Post</span>
            <p>
              A Quiet Haven<br />14 Quietwood Lane<br />Hackney, London E8
              3QD<br />United Kingdom
            </p>
            <span class="card-tag">Reply Times</span>
            <p>
              We answer letters and emails within a week, usually sooner. There
              is no automated reply, so silence simply means we have not reached
              your envelope yet.
            </p>
          </div>
        </div>
      </section>
    </main>

    <footer>
      <div class="container">
        <p>&copy; 2026 A Quiet Haven. Written with quiet care.</p>
      </div>
    </footer>

    <script src="script.js"></script>
  </body>
</html>

-- SCRIPT CODE #JAVA SCRIPT

/* =========================================================
   A Quiet Haven — script.js
   Vanilla JavaScript, DOM manipulation only. No frameworks,
   no build step, no modules. This single file is shared by
   all seven pages; every init/render function early-returns
   when its target elements are absent.
========================================================= */

/* ---------------------------------------------------------
   0. UTILITIES
--------------------------------------------------------- */
function qs(sel, ctx) {
  return (ctx || document).querySelector(sel);
}
function qsa(sel, ctx) {
  return Array.prototype.slice.call((ctx || document).querySelectorAll(sel));
}
function formatPrice(n) {
  return "£" + n.toFixed(2);
}

function escapeHtml(str) {
  return String(str)
    .replace(/&/g, "&amp;")
    .replace(/</g, "&lt;")
    .replace(/>/g, "&gt;")
    .replace(/"/g, "&quot;")
    .replace(/'/g, "&#39;");
}

function showToast(message) {
  var toast = qs("#toast");
  if (!toast) {
    toast = document.createElement("div");
    toast.id = "toast";
    toast.className = "toast";
    toast.setAttribute("role", "status");
    toast.setAttribute("aria-live", "polite");
    document.body.appendChild(toast);
  }
  toast.textContent = message;
  toast.classList.add("show");
  clearTimeout(showToast._t);
  showToast._t = setTimeout(function () {
    toast.classList.remove("show");
  }, 2400);
}

function setFieldError(input, message) {
  var field = input.closest(".field");
  if (!field) return;
  field.classList.add("error");
  var err = field.querySelector(".field-error");
  if (!err) {
    err = document.createElement("span");
    err.className = "field-error";
    field.appendChild(err);
  }
  err.textContent = message;
  input.setAttribute("aria-invalid", "true");
}

function clearFieldError(input) {
  var field = input.closest(".field");
  if (field) field.classList.remove("error");
  input.removeAttribute("aria-invalid");
}

function isValidEmail(v) {
  return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(v);
}

function validateRequired(input, msg) {
  if (!input.value || !input.value.trim()) {
    setFieldError(input, msg || "This field is required.");
    return false;
  }
  clearFieldError(input);
  return true;
}

function validateEmailField(input, msg) {
  if (!isValidEmail(input.value.trim())) {
    setFieldError(input, msg || "Enter a valid email address.");
    return false;
  }
  clearFieldError(input);
  return true;
}

function validateMinLength(input, min, msg) {
  if (!input.value.trim() || input.value.trim().length < min) {
    setFieldError(input, msg);
    return false;
  }
  clearFieldError(input);
  return true;
}

/* ---------------------------------------------------------
   0b. RESILIENT STORAGE
   localStorage is the primary store, exactly as intended.

   But when the site is opened by double-clicking rather than
   served, some browsers give every local file its own isolated
   origin. localStorage then still *works* on each page while
   being completely invisible to the next one, so a cart filled
   on shop.html reads back as empty on cart.html.

   window.name survives navigation within the same tab whatever
   the origin, so it is kept as a mirror and used whenever
   localStorage comes back empty. Nothing sensitive goes in it —
   only product ids, quantities, and which soundscape is playing.
--------------------------------------------------------- */
var MIRROR_PREFIX = "qh_state::";

function readMirror() {
  try {
    var raw = window.name || "";
    if (raw.indexOf(MIRROR_PREFIX) !== 0) return {};
    return JSON.parse(raw.slice(MIRROR_PREFIX.length)) || {};
  } catch (e) {
    return {};
  }
}

function writeMirror(obj) {
  try {
    window.name = MIRROR_PREFIX + JSON.stringify(obj);
  } catch (e) {}
}

function storageGet(key) {
  var value = null;
  try {
    value = localStorage.getItem(key);
  } catch (e) {}
  if (value !== null) return value;
  var mirror = readMirror();
  return Object.prototype.hasOwnProperty.call(mirror, key) ? mirror[key] : null;
}

function storageSet(key, value) {
  try {
    localStorage.setItem(key, value);
  } catch (e) {}
  var mirror = readMirror();
  mirror[key] = value;
  writeMirror(mirror);
}

/* ---------------------------------------------------------
   1. AMBIENT SOUND PLAYER
--------------------------------------------------------- */
var SOUND_STATE_KEY = "qh_sound_state_v1";
var audioEls = {};
var resumeListenerAttached = false;

function loadSoundState() {
  try {
    return JSON.parse(storageGet(SOUND_STATE_KEY)) || {};
  } catch (e) {
    return {};
  }
}

function saveSoundState(state) {
  storageSet(SOUND_STATE_KEY, JSON.stringify(state));
}

function writeTrackState(key, playing, time) {
  var s = loadSoundState();
  s[key] = { playing: playing, time: time || 0 };
  saveSoundState(s);
}

function seekWhenReady(audio, time) {
  if (!time) return;
  if (audio.readyState >= 1) {
    try {
      audio.currentTime = time;
    } catch (e) {}
  } else {
    audio.addEventListener(
      "loadedmetadata",
      function () {
        try {
          audio.currentTime = time;
        } catch (e) {}
      },
      { once: true },
    );
  }
}

function initSoundPlayer() {
  var buttons = qsa(".sound-btn[data-src]");
  if (!buttons.length) return;
  var state = loadSoundState();

  buttons.forEach(function (btn) {
    var src = btn.dataset.src;

    var audio = audioEls[src];
    if (!audio) {
      audio = document.createElement("audio");
      audio.loop = true; /* loops indefinitely; nothing stops it but its own button */
      audio.preload = "none";
      audio.src = src;
      audio.volume = 0.6;
      document.body.appendChild(audio);
      audioEls[src] = audio;
    }

    btn.setAttribute("aria-pressed", "false");

    audio.addEventListener("play", function () {
      btn.classList.add("active");
      btn.setAttribute("aria-pressed", "true");
      writeTrackState(src, true, audio.currentTime);
    });

    audio.addEventListener("pause", function () {
      btn.classList.remove("active");
      btn.setAttribute("aria-pressed", "false");
      writeTrackState(src, false, audio.currentTime);
    });

    audio.addEventListener("error", function () {
      btn.disabled = true;
      btn.classList.remove("active");
      btn.setAttribute("aria-pressed", "false");
      btn.title =
        "This soundscape is not available yet — add " +
        src +
        " to the media folder.";
      writeTrackState(src, false, 0);
    });

    btn.addEventListener("click", function () {
      if (audio.paused) {
        seekWhenReady(audio, (loadSoundState()[src] || {}).time);
        var playing = audio.play();
        if (playing && playing.catch) playing.catch(function () {});
      } else {
        audio.pause();
      }
    });

    if (state[src] && state[src].playing) {
      seekWhenReady(audio, state[src].time);
      var resumed = audio.play();
      if (resumed && resumed.catch) {
        resumed.catch(function () {
          attachResumeOnInteraction();
        });
      }
    }
  });

  setInterval(function () {
    var s = loadSoundState();
    var dirty = false;
    Object.keys(audioEls).forEach(function (key) {
      var audio = audioEls[key];
      if (!audio.paused) {
        s[key] = { playing: true, time: audio.currentTime };
        dirty = true;
      }
    });
    if (dirty) saveSoundState(s);
  }, 1000);
}

function attachResumeOnInteraction() {
  if (resumeListenerAttached) return;
  resumeListenerAttached = true;

  var resume = function () {
    var state = loadSoundState();
    Object.keys(audioEls).forEach(function (key) {
      var audio = audioEls[key];
      if (audio.paused && state[key] && state[key].playing) {
        seekWhenReady(audio, state[key].time);
        var p = audio.play();
        if (p && p.catch) p.catch(function () {});
      }
    });
    document.removeEventListener("click", resume);
    document.removeEventListener("keydown", resume);
    document.removeEventListener("touchstart", resume);
  };

  document.addEventListener("click", resume, { once: true });
  document.addEventListener("keydown", resume, { once: true });
  document.addEventListener("touchstart", resume, { once: true });
}

/* ---------------------------------------------------------
   2. PRODUCT DATA
  
--------------------------------------------------------- */
var LETTERS = [
  {
    id: "love-letter",
    name: "Love Letter",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/love-letter.jpg",
    description:
      "Bound in muted dusty-rose silk ribbon and sealed with rich golden wax over stacked vintage manuscript paper. An intimate confession, written slowly and meant to be kept.",
  },
  {
    id: "love-letter-1",
    name: "Love Letter I",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/love-letter-1.jpg",
    description:
      "Tied with natural twine, laid alongside dried lavender, and stamped with a deep crimson floral wax seal. Warm, earthy, and quietly timeless.",
  },
  {
    id: "romantic-letter",
    name: "Romantic Letter",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/romantic-letter.jpg",
    description:
      "A soft sage-green envelope dressed with real dried baby's breath and closed with a rose-gold heart wax seal. For the tenderness that doesn't need announcing.",
  },
  {
    id: "random-letter",
    name: "Random Letter",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/random-letter.jpg",
    description:
      "Let fate choose. One letter drawn at random from the full collection — love, comfort, romance, or catch-up — sealed before even we know which one found you.",
  },
  {
    id: "comfort-letter",
    name: "Comfort Letter",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/comfort-letter.jpg",
    description:
      "Written in sweeping copperplate calligraphy on warm ivory parchment and closed with a blush wax monogram. A steadying hand on the shoulder, in written form.",
  },
  {
    id: "catchup-letter",
    name: "Catch-up Letter",
    category: "Buy a Letter",
    price: 5.0,
    image: "media/catchup-letter.jpg",
    description:
      "A dusty pink textured envelope with subtle botanical embossing and a velvet ribbon. Reading it feels like tea with an old friend after years apart.",
  },
];

var STATIONERY = [
  {
    id: "calligraphy-paper",
    name: "Special Calligraphy Paper",
    category: "Start a Letter",
    price: 3.0,
    unit: "per sheet",
    image: "media/calligraphy-paper.jpg",
    description:
      "Heavy-weight deckle-edged cotton paper, milled to hold dipping inks and fountain pens without bleeding or feathering.",
  },
  {
    id: "calligraphy-pen",
    name: "Fine Calligraphy Pen & Ink",
    category: "Start a Letter",
    price: 10.0,
    image: "media/calligraphy-pen.jpg",
    description:
      "A lacquered pen balanced for both fine hairlines and generous swells, paired with a pot of archival-grade ink that dries true and dark.",
  },
  {
    id: "classic-envelope",
    name: "Classic White Envelope",
    category: "Start a Letter",
    price: 1.0,
    image: "media/classic-envelope.jpg",
    description:
      "A crisp, high-density envelope with a clean geometric flap and a softly lined interior. 184mm × 133mm.",
  },
  {
    id: "envelope-gold-seal",
    name: "White Envelope, Golden Rose Wax Seal",
    category: "Start a Letter",
    price: 5.0,
    image: "media/envelope-gold-seal.jpg",
    description:
      "A fine ivory envelope with a metallic gold rose wax stamp already pressed to the flap, so all that remains is the writing. 184mm × 133mm.",
  },
  {
    id: "rose-wax-stamp",
    name: "Crimson Rose Wax Stamp",
    category: "Start a Letter",
    price: 1.0,
    image: "media/rose-wax-stamp.jpg",
    description:
      "A self-adhesive wax seal in deep crimson, struck with a full-bloom rose and formulated to stay supple through postal sorting.",
  },
];

var DIGITAL = [
  {
    id: "digital-comfort",
    name: "Printable Comfort Letter",
    category: "Digital Letter",
    price: 4.0,
    image: "media/digital-comfort.jpg",
    description:
      "An instantly downloadable comfort letter template, ready to print at home and finish in your own hand tonight.",
  },
  {
    id: "digital-love-archive",
    name: "Digital Love Letter Archive",
    category: "Digital Letter",
    price: 6.0,
    image: "media/digital-love-archive.png",
    description:
      "Five printable love letter templates in our signature literary layout, bundled together as one downloadable archive.",
  },
  {
    id: "digital-stationery-set",
    name: "Vintage Stationery Sheet Set",
    category: "Digital Letter",
    price: 3.5,
    image: "media/digital-stationery-set.png",
    description:
      "Six printable letterhead and border designs, ornamental without being loud — run them through your printer before you begin.",
  },
  {
    id: "digital-grief-template",
    name: "Grief & Healing Letter",
    category: "Digital Letter",
    price: 4.0,
    image: "media/digital-grief-template.png",
    description:
      "A gently guided template for writing to someone you have lost, or to a version of yourself you are still quietly grieving.",
  },
  {
    id: "digital-historical-archive",
    name: "Historical Letters Archive Vol. I",
    category: "Digital Letter",
    price: 8.0,
    image: "media/digital-historical-archive.png",
    description:
      "A curated digital collection of correspondence styles drawn from letters past, for the writer who likes a little history in the ritual.",
  },
  {
    id: "digital-envelope-liners",
    name: "Printable Envelope Liner Set",
    category: "Digital Letter",
    price: 3.0,
    image: "media/digital-envelope-liners.jpg",
    description:
      "Eight botanical envelope liner designs, cut-ready for standard sizes — a private detail only the person opening it will ever find.",
  },
];

var ALL_PRODUCTS = LETTERS.concat(STATIONERY, DIGITAL);

function findProduct(id) {
  for (var i = 0; i < ALL_PRODUCTS.length; i++) {
    if (ALL_PRODUCTS[i].id === id) return ALL_PRODUCTS[i];
  }
  return null;
}

function categoryTagClass(category) {
  if (category === "Buy a Letter") return "tag-letters";
  if (category === "Start a Letter") return "tag-stationery";
  return "tag-digital";
}

/* ---------------------------------------------------------
   3. SHOPPING CART
--------------------------------------------------------- */
var CART_KEY = "qh_cart_v1";

function getCart() {
  try {
    var raw = JSON.parse(localStorage.getItem(CART_KEY));
    return Array.isArray(raw) ? raw : [];
  } catch (e) {
    return [];
  }
}

function saveCart(cart) {
  try {
    localStorage.setItem(CART_KEY, JSON.stringify(cart));
  } catch (e) {}
  updateCartCount();
}

function addToCart(id, qty) {
  qty = qty || 1;
  var cart = getCart();
  var existing = null;
  for (var i = 0; i < cart.length; i++) {
    if (cart[i].id === id) existing = cart[i];
  }
  if (existing) existing.qty += qty;
  else cart.push({ id: id, qty: qty });
  saveCart(cart);
  var p = findProduct(id);
  showToast((p ? p.name : "Item") + " added to your cart");
}

function removeFromCart(id) {
  saveCart(
    getCart().filter(function (i) {
      return i.id !== id;
    }),
  );
  renderCartPage();
}

function changeQty(id, delta) {
  var cart = getCart();
  var item = null;
  for (var i = 0; i < cart.length; i++) {
    if (cart[i].id === id) item = cart[i];
  }
  if (!item) return;
  item.qty += delta;
  if (item.qty <= 0)
    saveCart(
      cart.filter(function (i) {
        return i.id !== id;
      }),
    );
  else saveCart(cart);
  renderCartPage();
}

function cartTotal() {
  return getCart().reduce(function (sum, i) {
    var p = findProduct(i.id);
    return sum + (p ? p.price * i.qty : 0);
  }, 0);
}

function cartItemCount() {
  return getCart().reduce(function (n, i) {
    return n + i.qty;
  }, 0);
}

function updateCartCount() {
  qsa(".cart-count").forEach(function (el) {
    el.textContent = cartItemCount();
  });
}

/* ---------------------------------------------------------
   4. PRODUCT
--------------------------------------------------------- */
function buildProductCard(p) {
  var card = document.createElement("div");
  card.className = "product-card";
  card.innerHTML =
    '<div class="product-image">' +
    '<span class="product-tag ' +
    categoryTagClass(p.category) +
    '">' +
    escapeHtml(p.category) +
    "</span>" +
    '<img src="' +
    escapeHtml(p.image) +
    '" alt="' +
    escapeHtml(p.name) +
    '" loading="lazy">' +
    "</div>" +
    '<div class="product-body">' +
    '<span class="product-cat">' +
    escapeHtml(p.category) +
    "</span>" +
    '<h3 class="product-title">' +
    escapeHtml(p.name) +
    "</h3>" +
    '<p class="product-desc">' +
    escapeHtml(p.description) +
    "</p>" +
    '<div class="product-footer">' +
    '<span class="product-price">' +
    formatPrice(p.price) +
    (p.unit ? " <small>" + escapeHtml(p.unit) + "</small>" : "") +
    "</span>" +
    '<button type="button" class="buy-btn" data-buy-id="' +
    escapeHtml(p.id) +
    '">Purchase Item</button>' +
    "</div>" +
    "</div>";
  return card;
}

function renderProductGrid(containerId, products) {
  var container = document.getElementById(containerId);
  if (!container) return;

  container.innerHTML = "";
  products.forEach(function (p) {
    container.appendChild(buildProductCard(p));
  });

  container.addEventListener("click", function (e) {
    var btn = e.target.closest("[data-buy-id]");
    if (!btn) return;
    addToCart(btn.dataset.buyId, 1);
    btn.textContent = "Received ✓";
    btn.classList.add("added");
    clearTimeout(btn._resetTimer);
    btn._resetTimer = setTimeout(function () {
      btn.textContent = "Purchase Item";
      btn.classList.remove("added");
    }, 1400);
  });
}

/* ---------------------------------------------------------
   5. CART PAGE
--------------------------------------------------------- */
var SHIPPING_FLAT = 3.5;

function renderCartPage() {
  var list = document.getElementById("cart-list");
  if (!list) return; /* not the cart page */

  var cart = getCart();
  var emptyEl = document.getElementById("cart-empty");
  var layoutEl = document.getElementById("cart-layout");

  if (cart.length === 0) {
    if (layoutEl) layoutEl.style.display = "none";
    if (emptyEl) emptyEl.style.display = "block";
    setSummary(0, 0);
    return;
  }

  if (layoutEl) layoutEl.style.display = "grid";
  if (emptyEl) emptyEl.style.display = "none";

  list.innerHTML = "";
  cart.forEach(function (item) {
    var p = findProduct(item.id);
    if (!p) return;
    var row = document.createElement("div");
    row.className = "cart-item";
    row.innerHTML =
      '<img src="' +
      escapeHtml(p.image) +
      '" alt="' +
      escapeHtml(p.name) +
      '">' +
      '<div class="cart-item-info">' +
      '<span class="cat">' +
      escapeHtml(p.category) +
      "</span>" +
      "<h3>" +
      escapeHtml(p.name) +
      "</h3>" +
      '<span class="unit-price">' +
      formatPrice(p.price) +
      (p.unit ? " " + escapeHtml(p.unit) : "") +
      "</span><br>" +
      '<button type="button" class="cart-remove" data-remove="' +
      escapeHtml(p.id) +
      '">Remove</button>' +
      "</div>" +
      '<div class="qty-control">' +
      '<button type="button" data-dec="' +
      escapeHtml(p.id) +
      '" aria-label="Decrease quantity of ' +
      escapeHtml(p.name) +
      '">&minus;</button>' +
      "<span>" +
      item.qty +
      "</span>" +
      '<button type="button" data-inc="' +
      escapeHtml(p.id) +
      '" aria-label="Increase quantity of ' +
      escapeHtml(p.name) +
      '">&plus;</button>' +
      "</div>" +
      '<div class="cart-item-total">' +
      formatPrice(p.price * item.qty) +
      "</div>";
    list.appendChild(row);
  });

  setSummary(cartTotal(), SHIPPING_FLAT);
}

function setSummary(subtotal, shipping) {
  var subtotalEl = document.getElementById("cart-subtotal");
  var shippingEl = document.getElementById("cart-shipping");
  var totalEl = document.getElementById("cart-total");
  if (subtotalEl) subtotalEl.textContent = formatPrice(subtotal);
  if (shippingEl) shippingEl.textContent = formatPrice(shipping);
  if (totalEl) totalEl.textContent = formatPrice(subtotal + shipping);
}

function wireCartEvents() {
  var list = document.getElementById("cart-list");
  if (!list) return;
  list.addEventListener("click", function (e) {
    var inc = e.target.closest("[data-inc]");
    var dec = e.target.closest("[data-dec]");
    var rem = e.target.closest("[data-remove]");
    if (inc) changeQty(inc.dataset.inc, 1);
    else if (dec) changeQty(dec.dataset.dec, -1);
    else if (rem) removeFromCart(rem.dataset.remove);
  });
}

function initCheckoutForm() {
  var form = document.getElementById("checkout-form");
  if (!form) return;

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    var name = document.getElementById("checkout-name");
    var email = document.getElementById("checkout-email");
    var address = document.getElementById("checkout-address");

    var validName = validateRequired(name, "Enter the recipient's name.");
    var validEmail =
      validateRequired(email, "Enter your email.") &&
      validateEmailField(email, "Enter a valid email address.");
    var validAddress = validateRequired(address, "Enter a delivery address.");
    if (!(validName && validEmail && validAddress)) return;

    saveCart([]);
    var list = document.getElementById("cart-list");
    if (list) list.innerHTML = "";
    setSummary(0, 0);

    form.reset();
    form.style.display = "none";

    var success = document.getElementById("checkout-success");
    if (success) success.classList.add("show");
  });
}

/* ---------------------------------------------------------
   6. SELL A LETTER — writer application
--------------------------------------------------------- */
function initSellForm() {
  var form = document.getElementById("sell-form");
  if (!form) return;

  var fileInput = document.getElementById("writer-photo");
  var fileLabel = document.getElementById("writer-photo-label");
  if (fileInput && fileLabel) {
    fileInput.addEventListener("change", function () {
      fileLabel.textContent = fileInput.files.length
        ? fileInput.files[0].name
        : "Choose a file...";
    });
  }

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    var name = document.getElementById("writer-name");
    var email = document.getElementById("writer-email");
    var specialty = document.getElementById("writer-specialty");
    var excerpt = document.getElementById("writer-excerpt");

    var validName = validateRequired(name, "Tell us your name.");
    var validEmail =
      validateRequired(email, "Enter your email.") &&
      validateEmailField(email, "Enter a valid email address.");
    var validSpecialty = validateRequired(
      specialty,
      "Choose a writing specialty.",
    );
    var validExcerpt = validateMinLength(
      excerpt,
      40,
      "Share at least a few sentences (40+ characters).",
    );

    if (!(validName && validEmail && validSpecialty && validExcerpt)) return;

    form.reset();
    if (fileLabel) fileLabel.textContent = "Choose a file...";
    form.style.display = "none";

    var success = document.getElementById("sell-success");
    if (success) success.classList.add("show");
  });
}

/* ---------------------------------------------------------
   7. HOMEPAGE — Open a Letter / Leave a Note / Newsletter
--------------------------------------------------------- */
var SAMPLE_LETTERS = [
  {
    msg: "You do not have to carry the whole weight of the sky today. Soften your shoulders, breathe, and know that you are allowed to simply rest.",
    from: "A stranger, somewhere",
  },
  {
    msg: "You are exactly where you need to be right now, even if it does not feel that way from the inside.",
    from: "A stranger in Lisbon",
  },
  {
    msg: "Grief is only love with nowhere left to go. Be patient with yours; it is proof of something good.",
    from: "A stranger in Toronto",
  },
  {
    msg: "You have survived every single one of your worst days. That is not a small thing, and it was not luck.",
    from: "A stranger in Manila",
  },
  {
    msg: "It is allowed to outgrow people you loved deeply. Leaving gently is still a kind of love.",
    from: "A stranger in Berlin",
  },
  {
    msg: "Your softness is not a weakness. It is the rarest thing you own, and the world is quietly short of it.",
    from: "A stranger in Nairobi",
  },
  {
    msg: "Rest is not a reward you have to earn first. You are permitted to stop before you are finished.",
    from: "A stranger in Dublin",
  },
  {
    msg: "Somebody once sat exactly where you are sitting and made it through. Tonight, let that be enough.",
    from: "A stranger in Valparaíso",
  },
  {
    msg: "You are not behind. You are simply walking a road that does not happen to be signposted.",
    from: "A stranger in Kyoto",
  },
];

function initOpenLetter() {
  var btn = document.getElementById("open-letter-btn");
  if (!btn) return;

  var msgEl = document.getElementById("letter-quote");
  var fromEl = document.getElementById("letter-byline");
  if (!msgEl || !fromEl) return;

  var lastIndex = 0;
  btn.addEventListener("click", function () {
    var idx = Math.floor(Math.random() * SAMPLE_LETTERS.length);
    if (idx === lastIndex) idx = (idx + 1) % SAMPLE_LETTERS.length;
    lastIndex = idx;
    var pick = SAMPLE_LETTERS[idx];
    msgEl.textContent = "“" + pick.msg + "”";
    fromEl.textContent = "— " + pick.from;
  });
}

function initNoteForm() {
  var form = document.getElementById("note-form");
  if (!form) return;

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    var msg = document.getElementById("note-message");
    if (
      !validateMinLength(
        msg,
        10,
        "Share at least a short sentence (10+ characters).",
      )
    )
      return;

    form.reset();

    var success = document.getElementById("note-success");
    if (success) success.classList.add("show");

    launchPaperAirplane(form, qs(".sidebar-brand img"));
  });
}

function initNewsletterForm() {
  var form = document.getElementById("newsletter-form");
  if (!form) return;

  var pills = qsa(".radio-pill", form);

  var syncPills = function () {
    pills.forEach(function (pill) {
      var input = pill.querySelector('input[type="radio"]');
      pill.classList.toggle("selected", !!(input && input.checked));
    });
  };

  qsa('input[name="tier"]', form).forEach(function (input) {
    input.addEventListener("change", syncPills);
  });
  syncPills();

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    var email = document.getElementById("newsletter-email");
    var validEmail =
      validateRequired(email, "Enter your email.") &&
      validateEmailField(email, "Enter a valid email address.");
    if (!validEmail) return;

    var checked = qsa('input[name="tier"]', form).filter(function (i) {
      return i.checked;
    })[0];
    var tier = checked ? checked.value : "Daily Reflections";

    form.reset();
    syncPills();

    var success = document.getElementById("newsletter-success");
    if (success) {
      success.textContent =
        "Thank you — your " + tier + " letters will begin arriving soon.";
      success.classList.add("show");
    }
  });
}

/* ---------------------------------------------------------
   8. DELIGHT
--------------------------------------------------------- */
function launchPaperAirplane(fromEl, toEl) {
  if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) return;
  if (!fromEl || !toEl) return;

  var from = fromEl.getBoundingClientRect();
  var to = toEl.getBoundingClientRect();
  var size = 40;

  var startX = from.left + from.width / 2 - size / 2;
  var startY = from.top + from.height / 2 - size / 2;
  var endX = to.left + to.width / 2 - size / 2;
  var endY = to.top + to.height / 2 - size / 2;

  var midX = (startX + endX) / 2 + (endX - startX) * 0.14;
  var midY =
    (startY + endY) / 2 - Math.max(130, Math.abs(endY - startY) * 0.55);

  var deg = function (ax, ay, bx, by) {
    return (Math.atan2(by - ay, bx - ax) * 180) / Math.PI;
  };
  var a0 = deg(startX, startY, midX, midY);
  var a1 = deg(startX, startY, endX, endY);
  var a2 = deg(midX, midY, endX, endY);

  var plane = document.createElement("img");
  plane.className = "paper-airplane";
  plane.src = "media/paper-airplane.svg";
  plane.alt = "";
  plane.setAttribute("aria-hidden", "true");
  document.body.appendChild(plane);

  var animation = plane.animate(
    [
      {
        transform:
          "translate(" +
          startX +
          "px, " +
          startY +
          "px) rotate(" +
          a0 +
          "deg) scale(1)",
        opacity: 1,
        offset: 0,
      },
      {
        transform:
          "translate(" +
          midX +
          "px, " +
          midY +
          "px) rotate(" +
          a1 +
          "deg) scale(0.8)",
        opacity: 1,
        offset: 0.5,
      },
      {
        transform:
          "translate(" +
          endX +
          "px, " +
          endY +
          "px) rotate(" +
          a2 +
          "deg) scale(0.25)",
        opacity: 0,
        offset: 1,
      },
    ],
    {
      duration: 1800,
      easing: "cubic-bezier(0.4, 0, 0.2, 1)",
      fill: "forwards",
    },
  );

  var cleanUp = function () {
    if (plane.parentNode) plane.parentNode.removeChild(plane);
  };
  animation.onfinish = cleanUp;
  animation.oncancel = cleanUp;

  setTimeout(cleanUp, 2600);
}

/* ---------------------------------------------------------
   9.
--------------------------------------------------------- */
document.addEventListener("DOMContentLoaded", function () {
  initSoundPlayer();
  updateCartCount();

  renderProductGrid("shop-grid", LETTERS);
  renderProductGrid("stationery-grid", STATIONERY);
  renderProductGrid("digital-grid", DIGITAL);

  renderCartPage();
  wireCartEvents();
  initCheckoutForm();

  initSellForm();

  initOpenLetter();
  initNoteForm();
  initNewsletterForm();
});


-- STYLE CODE #CSS

/* =========================================================
   A Quiet Haven — style.css
   Single shared stylesheet. Modern romantic Victorian:
   warm ivory paper, deep ink, wine / rose / sage / gold,
   disciplined hairline grids and generous whitespace.
========================================================= */

/* ---------------------------------------------------------
   1. DESIGN TOKENS
   Every colour used anywhere in the site traces back here.
--------------------------------------------------------- */
:root {
  /* Paper & ink */
  --paper:      #FAF3EA;   /* page background — warm ivory, not stark white */
  --paper-deep: #F1E6D6;   /* card / panel background, one shade deeper */
  --cream:      #FFFDF9;   /* lightest surface — hover highlight, card-on-card */
  --ink:        #2B211B;   /* primary text — warm near-black, softer than pure black */
  --ink-soft:   #5C4A3E;   /* secondary text, captions, muted copy */

  /* Accent trio — romantic, botanical, Victorian */
  --wine:       #6E2A38;   /* primary interactive accent — buttons, links, active states */
  --wine-deep:  #4E1D28;   /* pressed / darker wine, hover-on-hover */
  --rose:       #C98A93;   /* dusty rose — soft accents, "Buy a Letter" tag */
  --sage:       #93A382;   /* botanical green — "Start a Letter" tag, success tint */
  --gold:       #B9975B;   /* muted brass/gold — dividers, fleurons, seal accents, focus glow */

  /* Structural */
  --line:        rgba(43, 33, 27, 0.18);  /* soft hairline for grids/dividers */
  --line-strong: rgba(43, 33, 27, 0.38);  /* soundbar/sidebar borders, stronger structure */


  --shadow-soft:  0 2px 14px rgba(43, 33, 27, 0.08);
  --shadow-lift:  0 8px 22px rgba(43, 33, 27, 0.13);
  --shadow-panel: 0 2px 20px rgba(43, 33, 27, 0.10);
  --tint-sage:    rgba(147, 163, 130, 0.14);
  --scrim:        rgba(43, 33, 27, 0.55);

  --font-display: 'Playfair Display', Georgia, 'Times New Roman', serif;
  --font-body:    Georgia, 'Times New Roman', serif;
  --font-ui:      'Helvetica Neue', Helvetica, Arial, sans-serif;

  --sidebar-width: 220px;
  --soundbar-height: 54px;
}

/* ---------------------------------------------------------
   2. RESET & BASE
--------------------------------------------------------- */
*, *::before, *::after { box-sizing: border-box; }

html { -webkit-text-size-adjust: 100%; }

body {
  margin: 0;
  background: var(--paper);
  color: var(--ink);
  font-family: var(--font-body);
  font-size: 1rem;
  line-height: 1.75;
  padding-top: var(--soundbar-height);
  padding-right: var(--sidebar-width);
  overflow-x: hidden;
}

img { max-width: 100%; display: block; }

a { color: var(--wine); }

::selection { background: var(--rose); color: var(--ink); }


:focus-visible {
  outline: 2px solid var(--gold);
  outline-offset: 2px;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2.2rem;
}

main { display: block; }

section { padding: 2.6rem 0; }

/* ---------------------------------------------------------
   3. TYPOGRAPHY
--------------------------------------------------------- */
h1, h2, h3, h4 {
  font-family: var(--font-display);
  font-weight: 600;
  color: var(--ink);
  margin: 0 0 0.7rem;
  line-height: 1.25;
  letter-spacing: 0.1px;
}

h1 { font-size: clamp(2rem, 4.4vw, 3.15rem); font-weight: 700; line-height: 1.16; }
h2 { font-size: clamp(1.5rem, 2.8vw, 2.1rem); }
h3 { font-size: 1.2rem; }

p { margin: 0 0 1rem; }

.literary-italic {
  font-family: var(--font-body);
  font-style: italic;
  color: var(--ink-soft);
  font-size: 1.06rem;
  line-height: 1.85;
}

.eyebrow {
  display: block;
  font-family: var(--font-ui);
  font-size: 0.66rem;
  font-weight: 700;
  letter-spacing: 2.4px;
  text-transform: uppercase;
  color: var(--wine);
  margin-bottom: 0.9rem;
}
.eyebrow::before { content: "— "; }

.section-head { max-width: 62ch; margin-bottom: 1.8rem; }
.section-head p { color: var(--ink-soft); }

.measure { max-width: 60ch; }
.measure-tight { max-width: 48ch; }

/* ---------------------------------------------------------
   4.
--------------------------------------------------------- */
.ornament {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1.1rem;
  color: var(--gold);
  font-size: 1.15rem;
  margin: 2.75rem auto;
  max-width: 1200px;
  padding: 0 2.2rem;
}
.ornament::before,
.ornament::after {
  content: "";
  flex: 1;
  height: 1px;
  background: var(--line-strong);
}

/* Hero wax-seal watermark — homepage only, a single quiet signature moment. */
.hero { position: relative; overflow: hidden; }
.hero .container { position: relative; z-index: 1; }
.hero-watermark {
  position: absolute;
  top: 50%;
  right: 4%;
  transform: translateY(-50%);
  width: clamp(220px, 30vw, 400px);
  aspect-ratio: 1;
  object-fit: cover;
  opacity: 0.08;
  pointer-events: none;
  user-select: none;
  z-index: 0;

  -webkit-mask-image: radial-gradient(circle, var(--ink) 52%, transparent 72%);
  mask-image: radial-gradient(circle, var(--ink) 52%, transparent 72%);
}

/* ---------------------------------------------------------
   5. BUTTONS
--------------------------------------------------------- */
.btn {
  display: inline-block;
  background: var(--cream);
  color: var(--wine);
  border: 1.5px solid var(--wine);
  border-radius: 2px;
  padding: 0.85rem 1.7rem;
  font-family: var(--font-ui);
  font-size: 0.72rem;
  font-weight: 700;
  letter-spacing: 2px;
  text-transform: uppercase;
  text-decoration: none;
  cursor: pointer;
  text-align: center;
  transition: background 0.28s ease, color 0.28s ease, transform 0.2s ease, border-color 0.28s ease;
}
.btn:hover,
.btn:focus-visible {
  background: var(--wine);
  color: var(--cream);
}
.btn:active {
  transform: translateY(1px);
  background: var(--wine-deep);
  border-color: var(--wine-deep);
}
.btn-block { display: block; width: 100%; }

/* ---------------------------------------------------------
   6. AMBIENT SOUND BAR — fixed top, horizontally scrollable
--------------------------------------------------------- */
.soundbar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: var(--soundbar-height);
  background: var(--cream);
  border-bottom: 1.5px solid var(--line-strong);
  display: flex;
  align-items: center;
  gap: 0.55rem;
  padding: 0 1.2rem;
  overflow-x: auto;
  overflow-y: hidden;
  white-space: nowrap;
  z-index: 1200;
  scrollbar-width: thin;
}

.soundbar-label {
  font-family: var(--font-ui);
  font-size: 0.62rem;
  font-weight: 700;
  letter-spacing: 2.2px;
  text-transform: uppercase;
  color: var(--ink-soft);
  padding-right: 0.7rem;
  margin-right: 0.2rem;
  border-right: 1px solid var(--line);
  flex: none;
}

.sound-btn {
  flex: none;
  background: var(--cream);
  color: var(--wine);
  border: 1.5px solid var(--wine);
  border-radius: 2px;
  padding: 0.42rem 0.95rem;
  font-family: var(--font-ui);
  font-size: 0.62rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  text-transform: uppercase;
  cursor: pointer;
  transition: background 0.28s ease, color 0.28s ease, border-color 0.28s ease;
}
.sound-btn:hover,
.sound-btn:focus-visible { background: var(--wine); color: var(--cream); }
.sound-btn.active { background: var(--wine); color: var(--cream); border-color: var(--wine); }
.sound-btn.active:hover { background: var(--wine-deep); border-color: var(--wine-deep); }
.sound-btn:disabled {
  opacity: 0.35;
  text-decoration: line-through;
  cursor: not-allowed;
  background: var(--cream);
  color: var(--wine);
}

/* ---------------------------------------------------------
   7. SIDEBAR NAVIGATION — fixed right
--------------------------------------------------------- */
.sidebar {
  position: fixed;
  top: var(--soundbar-height);
  right: 0;
  bottom: 0;
  width: var(--sidebar-width);
  background: var(--cream);
  border-left: 1.5px solid var(--line-strong);
  padding: 1.9rem 1.15rem;
  overflow-y: auto;
  z-index: 1100;
}

.sidebar-brand { text-align: center; margin-bottom: 1.9rem; }
.sidebar-brand img {
  width: 74px;
  height: 74px;
  object-fit: contain;
  margin: 0 auto 0.75rem;
  border-radius: 50%;
}
.sidebar-brand .name {
  font-family: var(--font-display);
  font-size: 1.08rem;
  font-weight: 700;
  line-height: 1.3;
  color: var(--ink);
}
.sidebar-brand .tagline {
  font-family: var(--font-ui);
  font-size: 0.58rem;
  font-weight: 700;
  letter-spacing: 2.6px;
  text-transform: uppercase;
  color: var(--gold);
  margin-top: 0.35rem;
}

.sidebar nav { display: flex; flex-direction: column; gap: 0.3rem; }

.sidebar nav a {
  display: block;
  font-family: var(--font-ui);
  font-size: 0.66rem;
  font-weight: 700;
  letter-spacing: 1.7px;
  text-transform: uppercase;
  color: var(--wine);
  background: var(--cream);
  border: 1.5px solid transparent;
  border-radius: 2px;
  text-decoration: none;
  padding: 0.62rem 0.7rem;
  transition: background 0.28s ease, color 0.28s ease, border-color 0.28s ease;
}
.sidebar nav a:hover,
.sidebar nav a:focus-visible { background: var(--wine); color: var(--cream); border-color: var(--wine); }
.sidebar nav a.active { background: var(--wine); color: var(--cream); border-color: var(--wine); }

.cart-count {
  display: inline-block;
  min-width: 1.35em;
  padding: 0 0.35em;
  margin-left: 0.35em;
  background: var(--gold);
  color: var(--ink);
  border-radius: 2px;
  font-size: 0.62rem;
  text-align: center;
}

/* ---------------------------------------------------------
   8. GRID
--------------------------------------------------------- */
.grid,
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  border-top: 1px solid var(--line);
  border-left: 1px solid var(--line);
}

.card,
.product-card {
  border-right: 1px solid var(--line);
  border-bottom: 1px solid var(--line);
}

.card {
  background: var(--paper-deep);
  border-radius: 2px;
  padding: 1.7rem;
  box-shadow: var(--shadow-soft);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.card:hover { transform: translateY(-2px); box-shadow: var(--shadow-lift); }

.card--solo {
  border: 1px solid var(--line);
  max-width: 640px;
}

.card h3 { margin-bottom: 0.2rem; }

.card h3::after,
.product-title::after {
  content: "✦";
  display: block;
  text-align: center;
  color: var(--gold);
  font-size: 0.8rem;
  line-height: 1;
  margin: 0.5rem 0 0.85rem;
  font-weight: 400;
}

.card-tag {
  display: block;
  font-family: var(--font-ui);
  font-size: 0.6rem;
  font-weight: 700;
  letter-spacing: 1.8px;
  text-transform: uppercase;
  color: var(--ink-soft);
  margin-bottom: 0.6rem;
}

.card p { color: var(--ink-soft); }
.card .btn { margin-top: 0.6rem; }

.book-meta {
  font-family: var(--font-ui);
  font-size: 0.62rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  text-transform: uppercase;
  color: var(--wine);
  display: block;
  margin-bottom: 0.6rem;
}

/* ---------------------------------------------------------
   9. PRODUCT CARDS
--------------------------------------------------------- */
.product-card {
  background: var(--paper-deep);
  border-radius: 2px;
  display: flex;
  flex-direction: column;
  box-shadow: var(--shadow-soft);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.product-card:hover { transform: translateY(-2px); box-shadow: var(--shadow-lift); }

.product-image {
  position: relative;
  aspect-ratio: 4 / 3;
  overflow: hidden;
  background: var(--paper);
  border-bottom: 1px solid var(--line);
}
.product-image img { width: 100%; height: 100%; object-fit: cover; }

.product-tag {
  position: absolute;
  top: 0.7rem;
  left: 0.7rem;
  z-index: 2;
  font-family: var(--font-ui);
  font-size: 0.58rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  text-transform: uppercase;
  color: var(--ink);
  padding: 0.3rem 0.6rem;
  border-radius: 2px;
}
.tag-letters    { background: var(--rose); }
.tag-stationery { background: var(--sage); }
.tag-digital    { background: var(--gold); }

.product-body {
  padding: 1.35rem;
  display: flex;
  flex-direction: column;
  flex: 1;
}

.product-cat {
  font-family: var(--font-ui);
  font-size: 0.58rem;
  font-weight: 700;
  letter-spacing: 1.8px;
  text-transform: uppercase;
  color: var(--ink-soft);
  margin-bottom: 0.5rem;
}

.product-title {
  font-family: var(--font-display);
  font-size: 1.12rem;
  font-weight: 600;
  margin: 0;
  color: var(--ink);
}

.product-desc {
  color: var(--ink-soft);
  font-size: 0.92rem;
  line-height: 1.7;
  flex: 1;
}

.product-footer {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  gap: 0.7rem;
  margin-top: 1rem;
  padding-top: 1rem;
  border-top: 1px solid var(--line);
}

.product-price {
  font-family: var(--font-ui);
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  color: var(--ink);
  white-space: nowrap;
}
.product-price small {
  font-size: 0.6rem;
  letter-spacing: 1.2px;
  text-transform: uppercase;
  color: var(--ink-soft);
}

.buy-btn {
  background: var(--cream);
  color: var(--wine);
  border: 1.5px solid var(--wine);
  border-radius: 2px;
  padding: 0.65rem 1.1rem;
  font-family: var(--font-ui);
  font-size: 0.65rem;
  font-weight: 700;
  letter-spacing: 1.8px;
  text-transform: uppercase;
  cursor: pointer;
  width: 100%;
  transition: background 0.28s ease, color 0.28s ease, border-color 0.28s ease, transform 0.2s ease;
}
.buy-btn:hover,
.buy-btn:focus-visible { background: var(--wine); color: var(--cream); }
.buy-btn:active { transform: translateY(1px); }

.buy-btn.added {
  background: var(--sage);
  border-color: var(--sage);
  color: var(--cream);
}

/* ---------------------------------------------------------
   10. FORMS
--------------------------------------------------------- */
.field { margin-bottom: 1.15rem; }

.field label,
.form-label {
  display: block;
  font-family: var(--font-ui);
  font-size: 0.63rem;
  font-weight: 700;
  letter-spacing: 1.8px;
  text-transform: uppercase;
  color: var(--ink);
  margin-bottom: 0.45rem;
}

.field input[type="text"],
.field input[type="email"],
.field select,
.field textarea {
  width: 100%;
  font-family: var(--font-body);
  font-size: 0.95rem;
  color: var(--ink);
  background: var(--cream);
  border: 1px solid var(--line-strong);
  border-radius: 2px;
  padding: 0.72rem 0.85rem;
  transition: border-color 0.25s ease, border-width 0.25s ease;
}
.field textarea { min-height: 130px; resize: vertical; }

.field input::placeholder,
.field textarea::placeholder { color: var(--ink-soft); opacity: 0.75; }


.field input:focus,
.field select:focus,
.field textarea:focus {
  outline: none;
  border: 2px solid var(--wine);
  padding: calc(0.72rem - 1px) calc(0.85rem - 1px);
}

.field.error input,
.field.error select,
.field.error textarea {
  border: 2px dashed var(--wine);
  padding: calc(0.72rem - 1px) calc(0.85rem - 1px);
}

.field-error {
  display: none;
  font-family: var(--font-ui);
  font-size: 0.6rem;
  font-weight: 700;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--wine);
  margin-top: 0.45rem;
}
.field-error::before { content: "— "; }
.field.error .field-error { display: block; }

.form-success {
  display: none;
  background: var(--paper-deep);
  border: 1.5px solid var(--sage);
  border-radius: 2px;
  padding: 1.15rem 1.35rem;
  margin-bottom: 1.4rem;
  font-family: var(--font-body);
  font-style: italic;
  color: var(--ink);
  box-shadow: var(--shadow-soft);
}
.form-success.show { display: block; }


.radio-row { display: flex; flex-wrap: wrap; gap: 0.6rem; margin-bottom: 1.3rem; }

.radio-pill {
  display: inline-flex;
  align-items: center;
  background: var(--cream);
  color: var(--wine);
  border: 1.5px solid var(--wine);
  border-radius: 2px;
  padding: 0.6rem 1.1rem;
  font-family: var(--font-ui);
  font-size: 0.63rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  text-transform: uppercase;
  cursor: pointer;
  transition: background 0.28s ease, color 0.28s ease;
}
.radio-pill:hover { background: var(--wine); color: var(--cream); }
.radio-pill.selected { background: var(--wine); color: var(--cream); }
.radio-pill input { position: absolute; opacity: 0; width: 0; height: 0; }
.radio-pill:focus-within { outline: 2px solid var(--gold); outline-offset: 2px; }

.visually-hidden-input {
  position: absolute;
  width: 1px; height: 1px;
  padding: 0; margin: -1px;
  overflow: hidden;
  clip: rect(0 0 0 0);
  white-space: nowrap;
  border: 0;
}
.visually-hidden-input:focus-visible + .btn { outline: 2px solid var(--gold); outline-offset: 2px; }

.file-row { display: flex; align-items: center; gap: 0.9rem; flex-wrap: wrap; }
.file-row .btn { cursor: pointer; }

/* ---------------------------------------------------------
   11. CART
--------------------------------------------------------- */
.cart-empty {
  border: 1px solid var(--line);
  border-radius: 2px;
  background: var(--paper-deep);
  padding: 2.4rem;
  max-width: 640px;
  box-shadow: var(--shadow-soft);
}

.cart-layout { display: grid; grid-template-columns: 1fr; gap: 2rem; align-items: start; }

#cart-list {
  border-top: 1px solid var(--line);
  border-left: 1px solid var(--line);
  border-right: 1px solid var(--line);
}

.cart-item {
  display: grid;
  grid-template-columns: 84px 1fr;
  gap: 1rem;
  align-items: center;
  padding: 1.1rem;
  border-bottom: 1px solid var(--line);
  background: var(--paper-deep);
}

.cart-item > img {
  width: 84px;
  height: 84px;
  object-fit: cover;
  border: 1px solid var(--line);
  border-radius: 2px;
}

.cart-item-info .cat {
  display: block;
  font-family: var(--font-ui);
  font-size: 0.57rem;
  font-weight: 700;
  letter-spacing: 1.7px;
  text-transform: uppercase;
  color: var(--ink-soft);
}
.cart-item-info h3 {
  font-size: 1.02rem;
  margin: 0.2rem 0 0.25rem;
}
.cart-item-info .unit-price {
  font-family: var(--font-ui);
  font-size: 0.65rem;
  font-weight: 700;
  letter-spacing: 1.4px;
  color: var(--ink);
}

.cart-remove {
  background: none;
  border: none;
  padding: 0.35rem 0;
  font-family: var(--font-ui);
  font-size: 0.6rem;
  font-weight: 700;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--wine);
  cursor: pointer;
  text-decoration: underline;
}
.cart-remove:hover { color: var(--wine-deep); }

.qty-control {
  display: inline-flex;
  align-items: center;
  border: 1.5px solid var(--wine);
  border-radius: 2px;
  overflow: hidden;
  width: max-content;
}
.qty-control button {
  background: var(--cream);
  color: var(--wine);
  border: none;
  width: 2.1rem;
  height: 2.1rem;
  font-family: var(--font-ui);
  font-size: 0.85rem;
  font-weight: 700;
  cursor: pointer;
  transition: background 0.28s ease, color 0.28s ease;
}
.qty-control button:hover,
.qty-control button:focus-visible { background: var(--wine); color: var(--cream); }
.qty-control span {
  min-width: 2.3rem;
  text-align: center;
  font-family: var(--font-ui);
  font-size: 0.72rem;
  font-weight: 700;
  letter-spacing: 1.2px;
  color: var(--ink);
  background: var(--paper-deep);
  align-self: stretch;
  display: flex;
  align-items: center;
  justify-content: center;
  border-left: 1px solid var(--line);
  border-right: 1px solid var(--line);
}

.cart-item-total {
  font-family: var(--font-ui);
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 1.4px;
  color: var(--ink);
  text-align: right;
}


.cart-summary {
  background: var(--paper-deep);
  border: 1.5px solid var(--gold);
  border-radius: 2px;
  padding: 1.7rem;
  box-shadow: var(--shadow-panel);
}
.cart-summary h3 { margin-bottom: 1.1rem; }
.cart-summary h3::after { content: "✦"; display: block; text-align: left; color: var(--gold); font-size: 0.8rem; line-height: 1; margin: 0.45rem 0 0; }

.summary-row {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  padding: 0.6rem 0;
  border-bottom: 1px solid var(--line);
  font-family: var(--font-ui);
  font-size: 0.68rem;
  font-weight: 700;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-soft);
}
.summary-row span:last-child { color: var(--ink); }
.summary-row.total {
  border-bottom: none;
  border-top: 1.5px solid var(--gold);
  margin-top: 0.5rem;
  padding-top: 0.9rem;
  font-size: 0.8rem;
  color: var(--ink);
}

/* ---------------------------------------------------------
   12. FOOTER
--------------------------------------------------------- */
footer {
  border-top: 1px solid var(--line-strong);
  margin-top: 3rem;
  padding: 2.2rem 0;
  background: var(--cream);
}
footer p {
  margin: 0;
  font-family: var(--font-ui);
  font-size: 0.62rem;
  font-weight: 700;
  letter-spacing: 1.8px;
  text-transform: uppercase;
  color: var(--ink-soft);
}

/* ---------------------------------------------------------
   13. TOAST
--------------------------------------------------------- */
.toast {
  position: fixed;
  left: 50%;
  bottom: 1.6rem;
  transform: translate(-50%, 1.2rem);
  background: var(--ink);
  color: var(--paper);
  font-family: var(--font-ui);
  font-size: 0.63rem;
  font-weight: 700;
  letter-spacing: 1.6px;
  text-transform: uppercase;
  padding: 0.8rem 1.3rem;
  border-radius: 2px;
  box-shadow: var(--shadow-panel);
  opacity: 0;
  pointer-events: none;
  z-index: 2500;
  transition: opacity 0.3s ease, transform 0.3s ease;
  max-width: min(90vw, 420px);
  text-align: center;
}
.toast.show { opacity: 1; transform: translate(-50%, 0); }

/* ---------------------------------------------------------
   14. MOTION & DELIGHT
--------------------------------------------------------- */
.paper-airplane {
  position: fixed;
  z-index: 3000;
  pointer-events: none;
  width: 40px;
  height: 40px;
  top: 0;
  left: 0;
}

@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.001ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.001ms !important;
    scroll-behavior: auto !important;
  }
  .card:hover,
  .product-card:hover { transform: none; }
}

/* ---------------------------------------------------------
   15. RESPONSIVE
--------------------------------------------------------- */


@media (min-width: 480px) {
  .product-footer { flex-direction: row; align-items: center; justify-content: space-between; }
  .buy-btn { width: auto; }
}

@media (min-width: 560px) {
  .cart-item { grid-template-columns: 84px 1fr auto auto; gap: 1.2rem; }
  .cart-item-total { min-width: 5.5rem; }
}

@media (max-width: 899px) {
  body { padding-right: 0; }

  .sidebar {
    position: static;
    width: 100%;
    height: auto;
    border-left: none;
    border-bottom: 1.5px solid var(--line-strong);
    padding: 1.3rem 1.2rem;
    overflow: visible;
  }

  .sidebar-brand { margin-bottom: 1.1rem; }
  .sidebar-brand img { width: 58px; height: 58px; }

  .sidebar nav {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.5rem;
  }
  .sidebar nav a { padding: 0.55rem 0.85rem; }

  .container { padding: 0 1.4rem; }
  .ornament { padding: 0 1.4rem; }
  section { padding: 2rem 0; }
  .hero-watermark { opacity: 0.05; right: -6%; }
}

/* Cart splits into items summary. */
@media (min-width: 900px) {
  .cart-layout { grid-template-columns: 1.6fr 1fr; }
  .cart-summary { position: sticky; top: calc(var(--soundbar-height) + 1.5rem); }
}


