<template>
  <CardChangeAccountInfo
    :ctaLabel="$t('components.card-change-account-info.username.header-cta')"
    :ctaAriaLabel="
      $t('components.card-change-account-info.username.cta-aria-label')
    "
  >
    <div class="pb-1 space-y-4">
      <div class="flex items-center space-x-4">
        <h3 class="font-bold responsive-h3">
          {{ $t("components.card-change-account-info.username.header-cta") }}
        </h3>
      </div>
      <div class="flex flex-col lg:flex-row gap-4 lg:gap-8">
        <div class="flex flex-col w-full lg:w-1/2">
          <label for="new-username" class="font-bold responsive-h4"
            >{{
              $t("components.card-change-account-info.username.new-username")
            }}
            *</label
          >
          <input
            id="new-username"
            class="peer border border-light-text rounded-sm bg-transparent py-1 px-3 dark:border-dark-text"
            :placeholder="
              $t(
                'components.card-change-account-info.username.enter-new-username'
              )
            "
          />
        </div>
        <div class="flex flex-col w-full lg:w-1/2">
          <label for="password" class="font-bold responsive-h4"
            >{{
              $t("components.card-change-account-info.enter-password")
            }}
            *</label
          >
          <input
            id="password"
            class="peer border border-light-text rounded-sm bg-transparent py-1 px-3 dark:border-dark-text"
            :placeholder="
              $t('components.card-change-account-info.enter-your-password')
            "
          />
        </div>
      </div>
    </div>
  </CardChangeAccountInfo>
</template>
