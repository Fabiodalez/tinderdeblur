async function unblur() {
  // Fetch teasers data from Tinder API
  const teasers = await fetch("https://api.gotinder.com/v2/fast-match/teasers", {
    headers: {
      "X-Auth-Token": localStorage.getItem("TinderWeb/APIToken"),
      platform: "android",
    },
  })
  .then((res) => res.json())
  .then((res) => res.data.results);

  // Select the blurred teaser elements
  const teaserEls = document.querySelectorAll(
    ".Expand.enterAnimationContainer > div:nth-child(1)"
  );

  // Replace blurred images with unblurred versions
  teasers.forEach((teaser, index) => {
    const teaserEl = teaserEls[index];
    const teaserImage = `https://preview.gotinder.com/${teaser.user._id}/original_${teaser.user.photos[0].id}.jpeg`;
    teaserEl.style.backgroundImage = `url(${teaserImage})`;
  });
}

// Execute the unblur function
unblur();
